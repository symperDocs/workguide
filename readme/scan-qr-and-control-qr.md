---
description: Chidk
---

# Scan QR and Control QR

## Scan QR and Control QR

### Overview

Scan QR: allows Enduser to scan each barcode or scan barcodes by tour in numbered order, solving the problem of adding numbers in the table

Control QR: display control QR code at Enduser screen, allow to download code, share QR code / Barcode image

\


## Scan QR

### BA configs for Text input control Allow scanning QR code and Barcode

Step 1: Click on a text input control, section "Scan configuration", check the checkbox "Allow QR scanning"

Step 2: Section "Order of recording data"

* If the BA does not enter "order of data recording": in the input screen, the user must focus on each control to be scanned for scanning.
* If the BA enters "Data recording order" (enter an order number greater than 0) for each control to be scanned: in the input screen, the user can scan by tour according to the order number entered in each control.

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

Usecases about scanning in Enduser screen:

| Allow scanning QR | Order of data logging | System                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| ----------------- | --------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Check             | Do not enter          | <p>- In the input screen, next to the text input shows the scan icon</p><p>- Users must manually focus on each control that needs to be scanned for scanning</p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| Check             | Import                | <p>- In the input screen, next to the text input shows the scan icon</p><p>- Display scan icon Total of document => User clicks scan icon Total, the system automatically focuses on the text input to be scanned without the smallest data, and scans by tour (from outside to inside the table and keep running the tour in table until the user's focus goes out)</p><p>- If the table also has a control to be scanned with ordinal number entered, display the scan icon of the Table => The user clicks the table's scan icon, the system automatically focuses on the text input to be scanned without the smallest data, and scan according to the tour in the table</p> |
| No accumulation   | Import                | Display and use as normal text input control, do not display scan icon next to text input                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |

<figure><img src="https://lh4.googleusercontent.com/ZctLqEN1-JOZ4pLv5gvUf5Sh-ekHUIO43U3ToY3ET9TWWTjeVbYnJivLf5_0wQjPRMGejzXE86PVtoZH51E-txqiCK2jaY5FZdQdaDQvUw_eXPn4ZoH3TUFWBAJSWun_5m6uONtyVKyLpc6HErurtGs" alt=""><figcaption><p>Scan by each input box</p></figcaption></figure>

<figure><img src="https://lh6.googleusercontent.com/4Tf3DDkFyVfFhOnN2oGKFqteYFXlkvShZRKoKqJdmgKMW2woHx1H5j0r1sQ4NxR2ErD47-S476R_gsuqhwVfYdMsle5IqaTkkSTqsehs7ssIRxQOaWCk1DiFu_gdcSwiZIoS4vj-JJCs02STN6iGKXU" alt=""><figcaption><p>Scan by tour with the Total text icon</p></figcaption></figure>

<figure><img src="https://lh6.googleusercontent.com/oJxbxWlXPnL9ci2XPgNpu2LcHJgZpOgnceWpOQPYtaNpZhVdP7q3J8gzCaXkfz7ya4De1EslCb3H9LUrqh_TtYKQK_Sm4JFocxlzvaJRYMSShNAW0HjnUySK_RWRlBhZRJncBAWmBNZ03toxvx0RQm0" alt=""><figcaption><p>Scan by tour with Table's scan icon</p></figcaption></figure>

Usecase user breaks thread to rescan information

1. Breaking the flow in the tour the controls have been entered in the sequence number:After scanning the input text box to re-enter, automatically focus on the scan box immediately after (regardless of whether it contains information or not)

<figure><img src="https://lh5.googleusercontent.com/rvQM5afVys3IJt8XMZ5g6-DmZDVD5NCOoTPB1skYFcMqttyKDgkAamXzYViByODq4t2A5bOZNM3BgsOzi6NpO8FNYs2SFOUbIZf9SkLpgD6Cd5Y5oh2ATfBYGwCKDTBSVb6VcdulUoVxhNizqjqCd1Q" alt=""><figcaption></figcaption></figure>

2. Break the flow outside the tour in the control without entering the sequence number: After scanning the input text box to re-enter, the system stops, does not run the tour, the user must focus on the next input text box to restart the flow

<figure><img src="https://lh4.googleusercontent.com/bMVrCs4wLFeO7Ui9sMzmvcqA64cOU0gNFk-GfZQBbX601_LA7tB21ALV8d8ivJ-0jyCpoD-KFkr86Px_5bprBwEjavnnU5w3KBkitQyZHgGNvFlmFbwnvP6GRcyZCJ0h8LCkpvcu8TO1CFlUkElMpeY" alt=""><figcaption></figcaption></figure>

Usecase scans QR code or Barcode containing a lot of information, fills data in other controls

In the control receiving data, the BA writes the value formula (SQLite):

WITH split(word, str) AS (

&#x20;   SELECT '', '{control\_scan}' || '-'&#x20;

&#x20;   UNION ALL SELECT

&#x20;   substr(str, 0, instr(str, '-')),

&#x20;   substr(str, instr(str, '-')+1)

&#x20;   FROM split WHERE str!=''

)&#x20;

SELECT word FROM split WHERE word!='' limit 1 offset 0 ;&#x20;

// edit to get word according to index 0,1,2… at offset

// edit the - to the delimiters according to the customer's pattern to split the string

<figure><img src="https://lh3.googleusercontent.com/PtFzitTID_rxPL8QHArC7ioWRdXLVGwse_UnJNKEkvEIJ5k8sfJJJJmKPxyZx6lXC6x5r4MKFCajF1HXpGpoCwAG3Rfpk0qxOopI9qhfjuSzacDXmx7jU4sZ1q8EsOAwggpGEQs_TSCR4N_Q7ApTLi0" alt=""><figcaption></figcaption></figure>

### BA configs for Table control Allow accumulation when scanning in the table

Step 1: Click on a control table, in the "Scan configuration" section, select the "Allow additional lines" property and check the "Allow accumulation when scanning" checkbox.

(If the BA does not select "Allow adding rows", the table does not automatically add rows and cannot be added manually, entering the first row will not add a new line)

Step 2: Section "Group data by": allows to select multiple controls in the table to group (meaning will merge rows if the data in the selected controls overlap)\
Step 3: The "Additional controls" section: allows selecting multiple controls in the table (only showing Number and Percent controls) to accumulate the number of those controls

<figure><img src="https://lh3.googleusercontent.com/uWzFobuVosfMlh9zl2lEoshGrMI0pf680UAt4_Ouc6M_b2nM5ywekB1x85ztPxv7kGDbrhAQw2TiMh2PYPYFvt5Ibrg54ocLjJhChQwDcsxSvoWVTCxJGck3su3iwa7whr8AVKibvXwI-luIeAZJx0M" alt=""><figcaption></figcaption></figure>

Accumulation usecases in Enduser level:

| Group data by     | Controls stack up | How the system works                                                                                                                                                                                                                                                                      |
| ----------------- | ----------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Select 1 control  | Select 1 control  | <p>- The system checks for duplicate data with another row</p><p>- Aggregate -> accumulate by control according to new quantity + old quantity</p>                                                                                                                                        |
| Select 1 control  | Select n controls | <p>- The system checks for duplicate data with another row</p><p>- Aggregate -> accumulate by control according to new quantity + old quantity (in selected cumulative controls)</p>                                                                                                      |
| Select n controls | Select 1 control  | <p>- The system checks for duplicate data with another row</p><p>- Scan 1 control -> duplicate but have not accumulated -> scan for n controls -> new duplicates accumulate -> accumulate according to control according to new number + old number</p>                                   |
| Select n controls | Select n controls | <p>- The system checks for duplicate data with another row</p><p>- Scan 1 control -> duplicate but not accumulated -> scan for n next controls -> new duplicates accumulate -> accumulate according to control according to new number + old number (in selected cumulative controls)</p> |
| Select            | Not selected      | <p>- The system checks for duplicate data with another row</p><p>- Combine lines but do not accumulate, the number is the old number</p>                                                                                                                                                  |
| Not selected      | Select            | Do not merge, add new lines                                                                                                                                                                                                                                                               |

## Control QR

### BA config control QR

Step 1: BA drag the QrCode control to the canvas screen

Step 2: Click on the QrCode control on the canvas screen

Step 3: Configure properties for control QrCode

| Code type | Display Type              | Datatypes |
| --------- | ------------------------- | --------- |
| QR code   | QR code Model1 and Model2 | Text      |
| Barcode   | Code128                   | Text      |

<figure><img src="https://lh3.googleusercontent.com/KsAu2IHcFa3zjAkTIlR_i7hav5F_sNLGV2eVmJ_EcK4goe89c3rcs58khJN2PKznjHZH52ZbIkQ6MQ7p9U6ZFvONAlzUupAYBO54uUNTLizoc9ArAb20loZorI4oO1GFDZcKdRCRQTrqb6ibseb-oXI" alt=""><figcaption></figcaption></figure>

<figure><img src="https://lh3.googleusercontent.com/j8eNqI1CvcDtAUscDNi1kELV3wyfQAeuU000zr8qcaZjfCi4OEICcyauiXOhn5qLq9X9d00gyyD736QKHR5RMSwRtAEFXBI9l3JPoxuSMfVVer6UxN2lQQsnE-sPtEk5YBSdjP6z9owF-TvX4JNDZ0c" alt=""><figcaption></figcaption></figure>

Step 4: BA writes a value formula for the QR control to get input data, to display the code

<figure><img src="https://lh5.googleusercontent.com/afYLCwtFgpsUrRL-N1BUtYFG3q_-bGChXdgbZ4CMbigprv-MQ2Hj45OSryeKqPIyZm0rbPYwCVIY99VaOupB1gXRnsqR-9mzSVVT8PXB7W5olUYpSncBP14oEv5E5sk2v2YYv9-qUfAERJx2nf9Aa9I" alt=""><figcaption></figcaption></figure>

### Usecases of QR control on Enduser screen:

1. Control QR has not received input value: display only QR icon

<figure><img src="https://lh3.googleusercontent.com/MhHJzKKKd3tqoLwxrblqmqA-yTNZToQVM_ME2bAcw1fbsdHWN1ickWTuDHOP3Fyz6SRC3rA6Num_tXcoACLLhFvxWwKphJDsuoDCjwV-h_zoHDqTlG7KWSzH8LGgHC0o689bC8LYfpmZ0bRGnWdIL9A" alt=""><figcaption></figcaption></figure>

2. Control QR when receiving input values: display code according to the type of code configured QR code or Barcode

<figure><img src="https://lh6.googleusercontent.com/MPZs0FNRmG9aHlc1RA7r0QU9BTM9-r1IZckxZjMXQMyj9tYD46VylXaj5WxO7wL0_hJyONZPd0GorX5S5xivl8dqfCI1cWb45HsvlaJjng40nO37Y1ypzowXWis-7yXM4vz6O7F20h3eD4vIPrehlA4" alt=""><figcaption></figcaption></figure>

3. User clicks on the code => The system opens a popup displaying the code image, the code's information, and the image download function

<figure><img src="https://lh4.googleusercontent.com/sovrFtXmC15cdnwA5o4j61FiLTsk2Z2AaGFQYY3MMP2vliqMX5w_YXfpyBMgzyeI2KE0wuZ-DlLoOpfRtx2Rc_iD_ruLoLAB-7ZWPETnnXjSlBYhfWVZrJiYPVhXlBQ82gE4YnKHpmIckLo5IpfIwnM" alt=""><figcaption></figcaption></figure>

<figure><img src="https://lh4.googleusercontent.com/px4DsO18FNGNL8FjITAYMgKdB2Y5tYKtvGbJC7Z1DVVKN7kcMDtFtvZcqkj37IezOuEU-q8ibbgSDDf_QYPEDT6BEumhkzLli3YcIg4s7HdnQsoK65Hlxp8kPL1ZJpY-Ges3A0v20fJVnC7ccZJ7zVc" alt=""><figcaption></figcaption></figure>

Use case config QR control size in table:

BA click on Table control, Properties section, enter Line Height

\=> Enduser screen: display Code Image Height = Table Line Height

<figure><img src="https://lh5.googleusercontent.com/0mgJybPOhT-HNkUmakYHeWM2_PzKRUsexq5AANSTeruyFIwsNh9YXwqcBroc6dEMwI-yfZtA9uvfia2YG9MMolR_UuxUT_lH4fgpv2em6OCvvTh_eaLwfB6NodobhApB5Q9lSDhUUrS9wrq_Zye4VBo" alt=""><figcaption><p>QR control image before configuring Line Height in table</p></figcaption></figure>

<figure><img src="https://lh3.googleusercontent.com/10Gp71S2ivrzi1Jv0nET20Fs2CrHUPY1NjNlrSx7r9l_1K_xMGtl_olkeibv8wLAVkYtP8EZs8R7Dm-AoFfV75oZbxcSC0AzV9pv2gfa9RwC9j4GNwMtGkFzgmZzzR2n8YFy5wL3wltd-HPGKe5j_9A" alt=""><figcaption><p>Configure Line Height in table</p></figcaption></figure>

<figure><img src="https://lh3.googleusercontent.com/eMHboaU6LSJYJbYI8oKmfPLKU5BD5V3x1BMUIzTdIerIaPIv1tdAacLVykzEwdA6THZ0-BSMI75inYwtjqfG-bN4DBQPRvdKeC6WTb-6Gr-7LtQeAFTu60EdaBht-NTtSuo-e6zHqaYpBW5se1gZkVA" alt=""><figcaption><p>QR control image after configuring Line Height in table</p></figcaption></figure>
