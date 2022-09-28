# Data Connector

**DATA CONNECTOR**\
****[**https://docs.google.com/document/d/1Dd8y5IpKUHjloMalcWkyWrgjHVrkS8I3Zrgbm6xNK3U/edit#**](https://docs.google.com/document/d/1Dd8y5IpKUHjloMalcWkyWrgjHVrkS8I3Zrgbm6xNK3U/edit)****

**OVERVIEW**\
**How to connect data between Symper’s system and other systems without having to know how they are implemented? APIs are a simplified way to connect or share**&#x20;
----------------------------------------------------------------------------------------------------------------------------------------------------------------------

## **STEP TO CONFIG**

**API stands for application programming interface. APIs let Symper’s product or service communicate with other products and services without having to know how they’re implemented.**&#x20;

**B1: To add new a ‘api’ , user click to button** ![](https://lh4.googleusercontent.com/hO0k3hOaItVvpUMoqNfWa83ysb\_C65aBSU9TODUM2Lvkhx8Dtja84Q9g3-YkM3jKowSc75Zcm63ui\_Nk02lpdMPVIsR7VMDW9BBpGRGw8nEpz6tcR3jhcq9CMse\_nJV-QWd3ZlMT) **then fill in the information in sidebar**\
****

![](https://lh4.googleusercontent.com/0hzDAJVC4a5KdsfwQavIMX8SXDIcEGOWgGVH-t0-0a19T63yPscyUUb-vei-63rX\_JdKyxx44ENitTEPFnEW7VoGkRBKH\_AKSej9CaEsMNuXkUhqij80mt-LtOPAsFzy-QGJ\_NX1)

![](https://lh4.googleusercontent.com/QvZE633cT2eg7\_h\_rLKZWU9Y9J7O3u4JeV87\_acGViDdz4wjLxjKo1Cm4RbaIHuPhuVRFIHcPuul6R2zsH0M2Gr8-qLOpCNr0p6nksew28X0DBU77E0dO8RkMkF9k8BhCl4nE4aC)

**B2: Enter API’s information**

**Components of sidebar:**\
****

**1- API link input area**

**2- Configuration tabs**\
****\
****

![](https://lh5.googleusercontent.com/qE05nPtULgOgvvoHCVgSBlHP7uoqSWT1w-YxRExuvRp4bVRBrhCXun5cpfbBl2pFfrUdJXQXX0RgOXT3MhKU2IpbfhDVMWVA8qx\_hbqqy9lcrqUoz-7n0Kqb84OzdYHcVq2sL9aI)

**1 API including method and 1 URL. Methods are get, post , put, delete,... depending on the user’s purpose , the admin of that system will send the URL along with the method.**![](https://lh4.googleusercontent.com/lWldOdMLLquY0FRZmCxnvovF9FDSRpobl\_ZbsFTDMon-Ambrx5qdasnEajSHOCLoZCh-w-5bmlJLT8q8RK3h8NqkBkwV17sgg2hRP6LRzQHy81YEW81g7UMokYh1VomPFEC3Hcl8)

**If the user gets data from another system, the user(BA or Admin) selects GET and enters the URL in the input box next to it.**\
****

**Example, this is an API :**

**https://symper.vitto.vn/api/bills/filter?factory=VTG\&pageIndex=1\&pageSize=5**

* **After the sign ‘?’ are the parameters.**
* **Parameters are separated by &**
* **Each parameters is structured as : key = value**
* **Factory: system address of the link**
* **pageIndex: number of pages**
* **pageSize : number of rows in 1 page**

**In the input box, BA/Admin enters the part before ‘?’ , the part after ‘?’ used to enter in the configuration tabs : Params, Header or Body . Normally, user enter parameters in the Params tab, Header and Body tab will fill if the admin requests.**&#x20;

**Khóa: user enter key**

**Giá trị: user enter value**

![](https://lh6.googleusercontent.com/cPMahPLIh2JghK4jX8yWeGr6szzjCqjpvwoHA9RVgH38eEsX6dBor3gpNkui27IoswH1Z-rSzVw5X-yejSnKSUGLjgY5Fy4sGsrYaWha1zMjHL79HLgLJWJvccizBfz1G6kmrCb3)

**Note: when entering parameters**&#x20;

* **Need to enter the correct key ( factory, pageIndex, pageSize)**
* **After entering the parameter’s information , user deletes the part after ‘?’ on the link**
* **pageIndex and pageSize’s value can change**&#x20;

**Ex: In URL pageIndex = 1, pageSize = 5, user can change to pageSize = 500, pageIndex= {page} . If data has 10.000 rows, split 500 rows into one page, pageIndex’s value is customization.**

![](https://lh4.googleusercontent.com/wg3ex-JpQaWb1OhbQTPcHITT8XIxlq--sBtHXqkUmLXFH0orGjdTiDtjfsxtK1ly\_MCkV-3SZgxGTKzzTjD6SA5B3vaZLK\_i1bXLwSz-ZPYHjLATt-Ue8dz\_LvSxvFvBTCKKAJ\_O)

**After user enter all the information, click to** ![](https://lh5.googleusercontent.com/bnXmpjXfDanIy1Zup1l1tmDR0YJmkYnsPZ9MbAASo31-HcB8hDkIMA3RaowwYaHvGg68wm2Cec5Y3j8AoqVUcDK2slUyW-m0TetzNBCqsD5mkkA3RM05McM60MxSK8WZWx6SuR5z) **to run the data**

![](https://lh4.googleusercontent.com/w0H8Iv6WOy6QMXwXvpRjWzBVOmaNuI3d7r37SHzK0xvH9Vj\_IFp2XZjM\_FFIEw2B2VwQwSX\_zFGkGyR-G6V65gKqqpPzpV84VcnDB5MhZwZqgjrU2uTFzAA\_mAbl7pWI7qG\_XbXv)

**B3. Data connection to the system**

**Make data connection at “Ghi dữ liệu”, user enter information of storage data (Nơi lưu trữ ), how to connect (add new, update or overwrite)**

![](https://lh3.googleusercontent.com/X-oErEAD6H04Gibp09hheuQB16X\_\_3bs4Eo7S-e9Jus2xzQnj4mdFWS6JjS8yBohw3Z\_Rf6xh112odNewKfrUvqhy30sKKJ4EdcQfjjffN\_Sv\_EJ3sUUJSWp\_PRL4xS2rvgZxnKs)

**Add new (Thêm mới): add new data and don't change old data**

**Overwrite (Ghi đè): change old data according to new data**

**Update (Cập nhật): change old data to new data when the condition is satisfied.** \
****

**When updating, user clicks to the check box to select the condition information field.**\
****

![](https://lh4.googleusercontent.com/4ovrnR3kSJ9PXT0FiH-TJBDvEC8Kyh3F2RKGMwvOBE1Ta7IZSzVxjfrrXETigNiDpzFpkkJsEWvIMTld2zqtL1q2hXXCnI3KevnC9bNvy5QK7\_9Yas7z\_Uu8t3-aX7ZdyBql7akh)

**BA/Admin select the corresponding information fields**&#x20;

![](https://lh4.googleusercontent.com/UEjJfNfsf36ViBWVXp9-tNNnqSZW5wNHQgrO-HQUL1eh7hgKWa-w-EajEx\_YGeWa5Ry52PujV36jdOPtP43ws9biLGIDCfD9n04IOHVeKvAds5qmerjDyROE\_9UORr9cuOFGkf9S)

**B4. Set run periodically**

**Default to run manually**![](https://lh3.googleusercontent.com/deIRYX3ELw2vn2pGaXfO36rxDALy694FI-NYEZOdNNC22DPJe3xPw-QCq0NHAFiWrQN6\_kxpKy\_6UwXwa8GtKz8n5UQgM5llG09EZAm\_oKhA50EreDW9lN3m1XrL-G3RaeILO6mQ)

**When user select “Chạy định kỳ”, the time setting showed below** ![](https://lh6.googleusercontent.com/VjGNqQhSxHQmaXkPkz7ihGFC6\_ra-BTtAO3fG9isgT5x70\_hEF2g7vzap\_boO5BqtG4lJVdH4bwgOnOtP22dld3iIEFaa-IPJrQBaUsIAVo4yfuUynBfiTbDXml4Zhg2MB93rLEJ)****\
****
