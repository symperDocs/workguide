# Event Node

## Definition

Tasks and gateways are two of three flow elements, and Events also are one of the most important notation of BPMN process models. Let start with some basic principles for applying them. We already used Start events, intermediate events, and end events. Those three event types are catching and/or throwing events. Those notation below represent for all the supported event in BPMN, but Symper not yet support all of them.

|                       | **Start Event**                                                                                                                                                                      |                                                                                                                                                                                     |                                                                                                                                                                                     | **Intermediate Event**                                                                                                                                                                |                                                                                                                                                                                       | **End Event**                                                                                                                                                                     |                                                                                                                                                                                     |                                                                                                                                                                                     |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|                       | **Standard**                                                                                                                                                                         | **Event sub-Process Interrupting**                                                                                                                                                  | **Event sub-Process Non-Interrupting**                                                                                                                                              | **Catching**                                                                                                                                                                          | **Boundary Interrupting**                                                                                                                                                             | **Boundary Non- Interrupting**                                                                                                                                                    | **Throwing**                                                                                                                                                                        | **Standard**                                                                                                                                                                        |
| **None**              | ![](https://lh3.googleusercontent.com/TL-lDgv4wCiE9Vxt2zVdKwc9Ezj87jEEq3LjswL2qmVcVLYf3r-RooJwlWprUtPVYmOBoU4kLCBF1tPeiRa4AFlFf30bSgv4iObi\_7HZwnV3KtgqwgUjNIGJykHF5a-U2TQqy7fj)     |                                                                                                                                                                                     |                                                                                                                                                                                     |                                                                                                                                                                                       |                                                                                                                                                                                       |                                                                                                                                                                                   | ![](https://lh6.googleusercontent.com/XDhQZ\_JbRfV1gNSYHVESD1bA7\_RhUnpPUmAed7tiOPIUhMPaUWSNqh8z5FoJze\_7k6lRaFjJSCNBAGXbI9P1NvNywdK4iWuYS7spGKltMUhI-Ppz0jippsJKkejyfJayqAUelYnK)  | ![](https://lh4.googleusercontent.com/RmXlW-dt3J50eqJoOIo979RF\_xknGuu6veEtiQ6BY\_K8Ci1sDuk3OO6dGFdgtZMnEWuuOF1tfu5BX8SDcn3LTawOWOXuXp7ctJz4OqH7wkBxIsNbcDJR8rF-PKUyyzhgDYoh3b5f)   |
| **Message**           | ![](https://lh5.googleusercontent.com/7JGnCWE0\_JzrhMTArjJUEufyPtJ-9pTgmAdsL\_62N50c7hn8Y6yzQXRnpRGZHa96HQqlHauaDc7oVG9nyOAwPgFOAhABFBjuLUppUR1maUwqyWCpxN8Q7lFEPW4DzBa8N-mxnZvD)    | ![](https://lh5.googleusercontent.com/Zm7LHTcISGuveonfXRpGRTTmfAnPJTZPp3rdfzjzm09cC4HqzDkLQXnqCVOJsQKPxTKYmzikn3YIx5ycfYAaPlrpxvSxTeOClqqmqAxUrHHi3dgMvHYYqF4em8EpXblIHpwNToWy)     | ![](https://lh3.googleusercontent.com/YdX1sn434e\_BrmIcvSJFEE1MK0NXRzLIKQkgmqbVs6yi9NeTheJdReTQnuSxubKpjQVtUaAazzuNCb49nGSbkMjyd9YPO7ZuIG2DNMUCfordSghFlf6ZKlJoNT8dAxtXmznYavTK)    | ![](https://lh6.googleusercontent.com/XTbP5TvOufWLO5WDKAiSBaJkHUwJgY-C8-mmaZ0g9-4AKb\_3ULs9Zx\_1bb0-S0RSTZiFmT9QIWNcFr4kdAwU2jo57BWFAta\_i1y9DJIyjIhGw3GXeBCX8nv7-61ZyyMXYrSUGfrt)    | ![](https://lh6.googleusercontent.com/XTbP5TvOufWLO5WDKAiSBaJkHUwJgY-C8-mmaZ0g9-4AKb\_3ULs9Zx\_1bb0-S0RSTZiFmT9QIWNcFr4kdAwU2jo57BWFAta\_i1y9DJIyjIhGw3GXeBCX8nv7-61ZyyMXYrSUGfrt)    | ![](https://lh3.googleusercontent.com/jRil8LojjT4nYoy5kp5AIkzRNet8OhPYEA5S09OcdqNWJJaD7hJPRJSmBcdGPASUSZSZ47TRSa2oLKJiIXxciA2hbjpVqIzzHcObnV8d08mvpFzAN8hQbAyduBa7kk9TXObbJYRH)   | ![](https://lh6.googleusercontent.com/GMYJDMfm3qSyBz4OaCfgfQzNA3\_xEN9ka-YHhEgXHVIatSzN7VpmNpkMmlJSX1x2wtUoG4Qqrc6aUkh8-rT0x1R1iGtKb2tcVWWeDCb66oOwqewt9LDL\_GQvtpa-zP0ivPHK0JPg)   | ![](https://lh6.googleusercontent.com/2CZNO7k5kIHOqGPNgwYNCHivsnqnhTCKGX1sm9su0fRB6Iu8EFARjTiwbsDrQQr96wiA-kPmm8k1slmRNIoQMRK3zOm0zvUIgcqmnW9AjCZLlbaEJOVGoJwWXjmuUIMTjtOtxO4y)     |
| **Timer**             | ![](https://lh6.googleusercontent.com/5s44fXz75iQysmF15o5hyegyiIHTeqdKbAmEIW3UOF\_MfMphoOO56z0Z9f2PmfKYwcuJSH8-hk\_DJpkAV1jei96-CsoVleCk3wlaGn2odyLseQd6Zfkn9nVnxDjnj2-qRitoWUtK)    | ![](https://lh4.googleusercontent.com/PiaiIW327cF97pl1I9gUL97NXJ4YXHEE55P0V9pgtKZKgvhh1lB95ookmxXWcnWbWV66WcDeMvDw8pJ9ebV0hPks6WbHW-0UtdKe6arq4kFknkvNVAfoqt8rdCH58FEdYDDvMevc)     | ![](https://lh4.googleusercontent.com/b30P16wYLnJAVgDDhpW7EMFClZUoMabN3Wu6AQbuiX6JLgxN6ZVhfaUaYo3Af5w5O75Ov4trRTxNPGsRe0jxH0s5WzK\_KmbXBAlSpM0h8837q\_cr5PEhVJLnw58j0OK08QjEeRGb)   | ![](https://lh6.googleusercontent.com/oI2yABMxQ0g3t1iK1DBuRkA1nGQVa0CDVkiEw5LAFleD082g\_fpIGo\_13hYJmV9DdANu\_77t03ULJ5uXZ1\_oecgrNix5rgOBJSWU\_JLZ54GhpWl\_M8qYhQWf37ZmicHOZUwmjwTe) | ![](https://lh6.googleusercontent.com/oI2yABMxQ0g3t1iK1DBuRkA1nGQVa0CDVkiEw5LAFleD082g\_fpIGo\_13hYJmV9DdANu\_77t03ULJ5uXZ1\_oecgrNix5rgOBJSWU\_JLZ54GhpWl\_M8qYhQWf37ZmicHOZUwmjwTe) | ![](https://lh4.googleusercontent.com/9hIXYueFulyxW332\_u8xROskPt3FWavMML4GibxGS8LtiG6sNmvklS-0Tf-OKUv2kXsftSSEg65eyBbAkqlnshYto9B4XWu-lAagWlD5krY5W4nz21QqrxT-ObHMD3aHKjZv3uvk)  | ![](https://lh3.googleusercontent.com/j96h12lJvjyoh4JW-RsYMeDsqtwkpijdUIKGkzEXthd1nc\_D7zg4OCg0a5bwFsGo4C2xfwNTtH5QroqGIPNnwy4uy9DANkVFiCbhCCbmXTkPWV68Zy-bWBwtPDXEkd77d8ooDUU7)    |                                                                                                                                                                                     |
| **Escalation**        |                                                                                                                                                                                      | ![](https://lh5.googleusercontent.com/y1n4ujrNbEVMu9o46OKP1qgKqkTUfXo100JJnP456OHhdfIk\_466XcKB\_51Ie0wOynA764-pEXhuMlXlIh1ThCSXBU1EFd6mIz\_cR-W8Zlvjr9k6t72AcYkIhbSCAUxgNvJWk2A5)  | ![](https://lh5.googleusercontent.com/IA-0iz7WQvdbzVFg\_DeD3fyyMkW9TS5N7FwQt5iShr6TPLft9AXZS-A4tFRtZQe3c7TULZ09KLeq6YEmpWHAn0mxJ6jKajZ5tnq8br8gB9p\_DPk4eFnX1f9Pa32Pz9zexN\_nP-FA)  |                                                                                                                                                                                       | ![](https://lh3.googleusercontent.com/5ofuIZuREibvd0YUuOd4UgYN1SAfJBmFoxs-XkCEoj7o3tzpAULmnF546ksFJ7weumSzzp3n1JeZVvFlpn8-886hv0otzxdC3R9siGtPTo7FE3TmBkixcTQQopMiM99jvGgJbvMV)       | ![](https://lh6.googleusercontent.com/8Pci3ASnkUx1uAyXeUlzw4EqGZFAbv4hwtkMjWAh99Z-pfb1D1lSvR2sB-pxSXeohGyP4bRqPF7sw6SYJWK29POh9THGglIQjJ-rh5kJPglM5NXO9\_xIWY-q1\_burVsbrmC-VmSp) | ![](https://lh3.googleusercontent.com/A-94PFdbOrORImT2aNlePvMq-gx0fWZuDNSAojbifQEKDeTjqI2IhLP\_EAhwhwf5PyBVXLSiNrAYdRwyTIlkHpiJhH9FM0BqkrWSU92tuCP9Y1tYthqJE5LZyrCh86ujSf-k4evt)    | ![](https://lh5.googleusercontent.com/Ts45Myo7YMwpuQicrv9AGndmR7oEYc\_02p0pIDgyY-8EoJ0PNmMszedekuoiBEdrh4Iz7qMnkF\_CvY5gqEA6oqfKU7JuEgWVewf-TqDTrpjRdRNxZZvS0C9PGlSyz9K5rsXfgRYY)   |
| **Conditional**       | ![](https://lh5.googleusercontent.com/5gGIeKL\_ARMyK7ZWfm4GkUR-rYX4BQQoriQHitCUz54VGwytoNyZVYeVLxrhbVhd38u3pnNI1mXS6TwWTQ1vcLzD5Uj3MPcjWj7Y0J0dYC1VSyDvYsWLm-8B3HEumV4wYQy0KXXi)     | ![](https://lh4.googleusercontent.com/IdsQSMAnJC\_qm7lbPeWjS9LKUG2jsmxCnEiP-98OnMHYZP9xF7gjVT3MSIldp-d1V4rKMK\_hxZXgsDLZ4fdcAkb4V3i85l4qeNeQlILwBmrW5QO2JxxkToKOeJlnSXEq2kbBtFkd)   | ![](https://lh4.googleusercontent.com/vfVpsyQgzrKyvIIHZWbzQfgpQVbGmr-0FtBBl9SQrFvMQfWXvt\_vgVhLvLGbfG-t0ku2IZmxotlWCp-TfKAE1pyFR1Mcj2SoEMrxqCdC4j7o9MA6nXgW9A-QIwG\_T55r7djBffZK)   | ![](https://lh3.googleusercontent.com/AoWSvxvbWSLhKhyudNI3hnu6mHeB5m5gYyRqtzWGGzoDJfaTsieOncbz-JUr7YIty1OzRh3408nEmgK-HHzos0JmX2G114nR7AtCRuPrKvvEX-9t1t2kHcHrGIXdO43M31hfDSpJ)       | ![](https://lh6.googleusercontent.com/YvICFZdzoMBdEhQdC1EpyKONAO4D1Lwqr4BOf6sPO4XMjQ693LbReKO5gw3zset9QYyOUzLJ5SlUGA0CJ9y14WW2ZT1zpf1Uomc3K0EzHaoOA4yzPXJz-k9lfsYa04LBduqq8DAd)       | ![](https://lh5.googleusercontent.com/UhaBJ6aMd0unKD9-2nREJtnW\_vrBs9VyxMvTcZN5lC747cS5EwjM6fSoRff8ZcXEif\_1rsf2bcibJ53HQBsrQMNy1QOh85APwA07Sk4gSRUhi2wAuEX7XThyoXgg4FY9kbcAX1hX) |                                                                                                                                                                                     |                                                                                                                                                                                     |
| **Link**              |                                                                                                                                                                                      |                                                                                                                                                                                     |                                                                                                                                                                                     | ![](https://lh5.googleusercontent.com/7KF1dVUxCveQIhyBBrW9kxuNJ5OuIlhocNWS4eXwIBzFUodRGuo6p7qYePEQPLlUE1RZRAOEtw0WspZKxtfAs8eO\_ADEBweRAER\_VJX00-vNY3ZQkQlH\_CKJOjCr\_WA-NhwkqpwM)   |                                                                                                                                                                                       |                                                                                                                                                                                   | ![](https://lh6.googleusercontent.com/iI15yzIUcDezyf2GRf7jB\_faqGpNRTb0fwx\_5QX2kCn5vf\_K3NrBWueoMECiKMLunxOhRehJ\_vAN-lj8S2hDURWtM86qPcsiVzmQtu7MMYtmEKJvWpgB-S1Up7cxkk1mztdwdMAm) |                                                                                                                                                                                     |
| **Error**             |                                                                                                                                                                                      | ![](https://lh5.googleusercontent.com/pqJ1qL9Az5RLP7S7nrLyCUrFci092\_pbTmnPFRN8hFOeKsgash2jXnU8oCyMBznHifiwgO66MbaOlBs5L9kYZWrR0qnsPIsq45MO-75\_K8lwt5D3XgG\_bzTJ76PgBiJBsAFLQ3JH)  |                                                                                                                                                                                     |                                                                                                                                                                                       | ![](https://lh5.googleusercontent.com/kc3CKVPKnj9Sh2LRyG7SHLAHEtj\_cy0rIUp666yjB09WxOCcKbpgWRT3p11iB81E6LX4p5UlGeakSh50ww18x04GHPQgg7wiJjOg2GICgMjxg5puLL4YdodFZqOGKf0-BqeYgjmY)      |                                                                                                                                                                                   |                                                                                                                                                                                     | ![](https://lh5.googleusercontent.com/m-hexlKviPVs3fZEVVleRejVlbdiVKV3\_\_76VyAqMaXk2iuNH6C\_KyxNTsojh58tv2bd5pFxjq5WT0PXlfnLCakeKB-D9xAVooXZuOWoGuU38cDX39YM2iOc6UqcZMHXGVvy0kj-)  |
| **Cancel**            |                                                                                                                                                                                      |                                                                                                                                                                                     |                                                                                                                                                                                     |                                                                                                                                                                                       | ![](https://lh5.googleusercontent.com/cKBNQqsKWJp9yPsq0rA5BSVN-PqfVLuFvy03VTDeWbpYX4jxifzpCSLIXjpdOlHGKO-be1E1vvwu-S7G1fpx5KHuzy-RNHNeB7iPjciP6hAj27i3d8e1wPxNNQhyf-8E3h0i8nOw)       |                                                                                                                                                                                   |                                                                                                                                                                                     | ![](https://lh5.googleusercontent.com/\_f7Ycstup6Xq-n8RA6\_wNnjluecFJ\_LxkFL1F2MhjcOQmuShWVfG1deZWc0mIrsb5fTZprNrdwe5W74rWtWfElYXCvh0-gpBwVSnLtBGrIreg73KQkEa5c2hVX0PqJ9me580pVJz)  |
| **Compensation**      |                                                                                                                                                                                      | ![](https://lh3.googleusercontent.com/oWWX\_wGc0CpFFv\_79JkYdpxHnHk0qaHJpYKo1BBmkRep278RLHEJuOc7RFq3VldY-1kXhlNLema8OulTLM6CXZWDLB6SMSeEhqroBgZHzuWbDnVoPNLHuC31Fp\_KUo4omptWUhdv)  |                                                                                                                                                                                     |                                                                                                                                                                                       | ![](https://lh5.googleusercontent.com/um5YbzoYmu0WLDhdzGRWQUY9OrSrJHi-TMOepjaqLVMHHBop8HBaZ1vUNa0yRPTO8xSbmiQ4ektNnRToT1xuCkGQYnjL42Ihtnw0xHuypfr3CDLaua0VKZIowfbnB8ldLUEGt59K)       |                                                                                                                                                                                   | ![](https://lh4.googleusercontent.com/IE1IhrsISIiKBPtHnvmNjpw9\_0Ac7gtZ\_87G4RuUcJLJ11jGSdi4koil3WiGGuo1LFMu0xfsdy5P2XLbsgyPSOFwX5IO3YCKTN2LyuENRLLFO9Jt0hKrBVG7i2Vn-MSyug4Usm1v)   | ![](https://lh6.googleusercontent.com/5YiJNwjXpSSj\_da-Z4\_HtBzTdoPQ-zI\_QvRD0hSaMXnhjhYiuPEurq3j73O7WX38nqq2Z2WgSku87f8-q0yJXezkrmXtuRfwtbIbFvJL51uxMtlbF0QRZisF\_sNFsOAnNgLPjBK8) |
| **Signal**            | ![](https://lh4.googleusercontent.com/AvlVje1UIMZsZMEQEixzEZqFtBYQm9MBlQitq7xiwilEVL5rqNLUY-TiB2Ug6QC4qHmcV7xkkxgYYQ70JJoGYubbb28A7yjnffJi9XPDvgb71ZeCh69wFE1yvIvR6N6vhGtBtnv4)      | ![](https://lh3.googleusercontent.com/c3Hg8M-IukIqKTFQosg8WfLvov2HC4XQlxaaeow1dBULmpwfNecP1KSiBV1dA0UT5-jInCG5H\_n-TH4xelXY0bXTD1DqhCz\_onwk7OcZfRCdAdhm8\_qJHDEW8I1h31tQgKjaJnyJ)  | ![](https://lh6.googleusercontent.com/ZaruopJsMvXoA368kka5o6rki0sOqLB\_ur21lh0xfMlgjTEkn99AA2lkCabva\_srJl0FiY4RfAjUa5hQ6kVEQnh3mSm\_w-S80qpuBO35NGSATCef5EVxCzdwEqfnOGKR\_5TVdwM3) | ![](https://lh3.googleusercontent.com/x17XaJJCTtnI7-HibVrvw1duz5dcZXNztBEES5wLBNIAB7izxcW4Dwq89gQiw9Oz5vxD6rgwswdXVnySbkiZyOBAi4NaGFnfw4VH6--bBL\_VVfJcIJ7\_FYKQukStEgANXitdrbE9)     | ![](https://lh4.googleusercontent.com/7kBsMSVpz5NvLk8SxS9B2D7NF-8SvwjMD6Tzq56cemhxdszCLtPs1wsr7h5t1UE\_-U7NDibMq5Cc2pajq6qOb070LGHI3BmWVe4OLF91FsxmpPT4AYre\_5jau4k2M-zqq56\_LkfE)    | ![](https://lh3.googleusercontent.com/k6PQ64uTSB2I2\_4suHB-6URBQlo6vTXfx44dOnaSsLpeBo7EQ1d-G70ZRIicDTf-r5V2ikO4jiFzUhRcPpEl3PNtdfWJdfa3IySU4vYKQVCT1juYpZaTYMlppZ-RNOlAtpqKZLkw)  | ![](https://lh6.googleusercontent.com/WZQEz\_MBUsHGympoJ7F9qtSuT7zXnCjuqi-910NvsAsEmidC0YWaXJgnfRtYZ3gqpZdUlHRo1Hw9MndBjhZToxu-rThyqWQLWEcLaay2ioXWy-gaocKXTTFj0LDs2KwQx4qSnZ4D)    | ![](https://lh6.googleusercontent.com/ibV1dsnsGp6h3D\_itYYFK8YER1vxk-iwqCbitWbriUi\_4QeDW6mSjRMLhi1MKWQNDEb8j7ClUkCgYiB7e-yn4pVcGmn299pCyr53TNR8\_ZbDgF\_TNlEpMZT9K33X--Vyw9ROaPad) |
| **Multiple**          | ![](https://lh5.googleusercontent.com/\_UGB1uFmM6TIfTWyoCKaBOok\_dnnBXhmCvWWvkbdwRBze39yfdI64Xemeu0UJ-CNX-aydxCMCCn4Pbpjg8B1uh10bjwLVTj6vqpSS9sfQRxw2JmOCJnuAPA1I6UVCT5vgrsRufxu)    | ![](https://lh5.googleusercontent.com/6Ftk-lUDx4Kf8j-MQLQvEoIMpKiweSY-sspUVstRCgA0Nl-Ea0X0\_Drt5npHIwrWGMoUgaT1k40V1WP8aJLG16HRW8tK1-2bpLdrnNNvDogNbtvenhe9XsccvXKEUOlwOHRWWncm)    | ![](https://lh5.googleusercontent.com/nCqpLARJ5CFDXtmjl6BuxSMPXELhokGcKj-3Y2czRdw\_gKOE07zIvnGRVfKAu7Yj-w3inLrMljWbwJGPxbF\_cFz2ZQAdR23\_2qeeL9J5pN8wJ1yYh1M1cXBAAdtJ7yMQtamUlXpc)  | ![](https://lh5.googleusercontent.com/ZJGLeDkIchE2rYw-lab2a9HjMXVHkn7niGJq25TYZrjAmY-cmIbh9seMwpPIbk2H\_R2Mv4eTjAZy\_wrob4GCVNH1y8BEfKK1jS69eCBEqu9ljyGeLy6CANB\_HgCBV3T8YIt6JJvF)    | ![](https://lh4.googleusercontent.com/wO\_0pM8s2\_KPYc-R1fbYZ9FnJj4yq7stuqfSRQg\_uYHUsYt3DjM836pdsXlWpLsHqmjZrLLES8vCt-i5XUnfgxkYWmZu2wu\_oxCuRdGdGqbbKUpzghD98h7oZrjmmwzcABU9oXLM)   | ![](https://lh3.googleusercontent.com/NAhguvGyC553bfLc1FK7RFrKcORuVJRUS-eMGR0xsIwbOgBKVc3Ns0WU7n4vxr67c1t6UnxOPvDLw3cgeotnLyJloU0ZTgsgCylb3wxCZlkKJtsyiq0s12lm7f419PFANuQ1LsWP)   | ![](https://lh5.googleusercontent.com/1C6uoRao2mdwoPeiad6Z-zrkp6X7fI3yyTGMxNRjmNXJlcEaZx-Ku\_jdCNWfcgUlF\_hQiKDEDf\_2S2aIWu0fN0xgd22XDnarGvd0flHG5xh1LWLRZoBgpBepuwGq\_Ow1wZQ7GymA) | ![](https://lh5.googleusercontent.com/n6QBIZ8TDYVTQl2XNUUvo0NhFpYgDRqC0hXzNpTq00toLmNnvcsZ1zz6rbHNotOZIn2LgEnO\_gpXxE935yuyqSYsrJqtebn664KdHQkfpPfgun6cT7plTA7Of\_bbo5UJIVD0mfhb)   |
| **Parallel Multiple** | ![](https://lh5.googleusercontent.com/tRgVBMs3i00uQh0BqwC\_GiSN3GscWYBumr9M9a-hl9JBbaTpghcRnTm3FdEHojkzbjQZ91eSdqtqNK42JM\_B79NlfMKM8dQb3eE\_TQHv70\_2L2dNvpE1\_TgUuKuSzC2JfIEZCSPI) | ![](https://lh6.googleusercontent.com/y2vZj34Noqx0P5rDZBvMp4nDlORXcwB2fFbb6u7e4b\_p6kj3aNua\_81NMcAhx1cy7PX\_HSrONChhWg8g01ntwDXh\_0vgPZRdHrPg5VT19-zYcuyY9vlVWYaLY3jKziMX486Zh8my) | ![](https://lh4.googleusercontent.com/p\_b55kLxvVLaFckXyg7cVq5MbxMUaru-x3jZyX897x4Gip\_fGNvytKoJ013CZp-mPg2YZh8-WkGP1A5W65lsVBiV3x3kUnO0oR0XBFXTvgOVHx-m4gbE\_FjgvwC-XFxgpN\_lS4qK) | ![](https://lh6.googleusercontent.com/0\_XYQx6\_Mksj2ROB8FiU45opQwScPcLhGzT-S1fHsw2nVTw5Mn6tCm1\_IYfdwlNlJdbTxSDJ\_mUPEK5WDwkzjHJRGDYIoOFze7pdgeVF4x\_ED0a2bzTswGfdDPFPG0t2Ar6BB6GE)  | ![](https://lh6.googleusercontent.com/A0ZOyP-R4plqN0ZvDlbNCyhECSLINKyD4p4itXkIJl28qk-T\_JulShuyt2SeiYBpq-hE3hFSUersE65dbcD4fpma9TigPu44-K\_8I81K6E327gHvusA9jfXnqeXWdWGeg-qmLoQo)     | ![](https://lh6.googleusercontent.com/6VQLcVW5aMcko7HYUswAbHT11gmNmzoQ-bX1i6cGPOHhiu1yLTuUfsLm11CemaU7P1ntVYp\_yosx53dTcovLgFBulC5u2YMTo5ca38SqVgNZdRRZ4MONcS1L8ZESX8Lmbwyul7EG)  |                                                                                                                                                                                     |                                                                                                                                                                                     |
| **Terminate**         |                                                                                                                                                                                      |                                                                                                                                                                                     |                                                                                                                                                                                     |                                                                                                                                                                                       |                                                                                                                                                                                       |                                                                                                                                                                                   |                                                                                                                                                                                     | ![](https://lh3.googleusercontent.com/Bq\_rNpxIBY3cjgSjL8EnJLdR0UZHQPvugzN5WEk915Zz-l7W2c8PtDPjXAfLF2TCtk1ZIhFc31vZv0Cvjh4HBtSCNlgwgRHn5zkcsIdSF\_7i1twvRStz-uuuI-Jn3P0\_Ec7q5lcc)  |

## **Catching events**

**Catching events** are events with a defined trigger. We consider that they take place once the trigger has activated or fired. As an intellectual construct, that is relatively intricate, so we simplify by calling them catching events. The point is that these events influence the course of the process and therefore must be modeled. Catching events may result in:

* The process starting
* The process or a process path continuing
* The task currently processed or the sub-process being canceled
* Another process path being used while a task or a sub-process executes

## **Throwing events**

**Throwing events** are assumed by BPMN to trigger themselves instead of reacting to a trigger. You could say that they are active compared to passive catching events. We call them throwing events for short, because the process triggers them. Throwing events can be:

* Triggered during the process
* Triggered at the end of the process

We can also model attached intermediate events with BPMN. These do not explicitly require waiting, but they do interrupt our activities, both tasks and sub-processes. Such intermediate events are attached because we position them at the boundary of the activity we want to interrupt.

<figure><img src="../../../.gitbook/assets/image (1) (1) (3) (1).png" alt=""><figcaption></figcaption></figure>

A token running through the process would behave this way:

* The token moves to task 1, which starts accordingly.
* If event 1 occurs while task 1 is being processed, task 1 is immediately canceled, and the token moves through the exception flow to task 3.
* On the other hand, if event 1 does not occur, task 1 will be processed, and the token moves through the regular sequence flow to task 2.
* If event 1 occurs only after task 1 completes, it will be ignored.

With the exception of compensation events, attached intermediate events inevitably resulted in canceled activities. BPMN 2.0 defines a new symbol: the non-interrupting intermediate event.

<figure><img src="../../../.gitbook/assets/image (4) (3).png" alt=""><figcaption></figcaption></figure>

The token moves through the process as follows:

* The token moves to task 1, which starts accordingly.
* If event 1 occurs while task 1 is being processed, the token is cloned. Task 1 continues to be processed while the second token moves to task 3, which is now also processed. This procedure may even take place repeatedly, that is, the event can occur many times. Each occurrence results in another cloned token.
* If event 1 does **not** occur, task 1 will be completed, and the token moves through the regular sequence flow to task 2.
* If event 1 occurs only after task 1 completes, it ceases to matter.

In the following sections, we introduce the event types to be used when working with BPMN. We also explain how you can react to different events using the event-based gateway.\\

## Event Node in Symper System

* Start event node (first node for start workflow)
* Start event

Normal start workflow, when chose start a process instance

![](https://lh3.googleusercontent.com/A8aCH-UasE2E0C1kCRgIDn4QqTuZy-xy\_55Xf-y9YOk-l7HkkXD4bEEjIbMnTlAgQM57NIwf8b4QAVWnUT8FXspLFeYk4aNaeZ8fIfognYCl-XffD2UXDi\_vK-G43bWxq5rDF5\_N)

### **Config**

* Form reference: \*\*\*\* Select document, a submit task will be created and assign to initiator

![](https://lh3.googleusercontent.com/zpCbPqzIw4u\_w9HY3UKKxr\_n5xjIcCVQSYz4v\_VJ0spKo-\_hbVhuJMJXCFxuOVw9bjZ3YeOn\_a7ZXWNL16dP0INx83Xj-1r1QtNXsT9yU2MHQDgKvF73QHdG3sZUk7nZYR634IBd)

1. **Message event**

When process receives a message that has same message name from Throw message, process will be started

**Config:**

* Message reference: Choose message id of throw message node. You need to declare Message definition on the general right sidebar.

1. **Timer Start Event**

A start node can setup initial time for process instance

#### Config: (use crontab or ISO-8601)

* Time cycle (cron) : Specifies repeating intervals
* Time date in ISO-8601 : Set start time at a point in time
* Time duration: To specify how long the timer should run before it is fired

1. Conditional Start Event

Set a formula or expression using SYQL as a condition to start workflow.

#### Config:

* Conditional expression: set a condition only when all conditions are met, the process instance starts.

1. Signal Start Event

This node will start a process when catch a signal from Throw signal has the same signal ID

#### Config:

* Signal reference : Select Signal name (Need to declare signal definition on the general right sidebar)

![](https://lh5.googleusercontent.com/R2TzsglT4Khn4aEHKj0nnA2lPSasYHhKIMt\_Kh5abJSH4ibsnlMUHa0o2Sz1JsV0zIg6cj73A-1OK0iZTRj-XFFKmec1NogPW6BmDSWNN3YcUZ013e3SLEHLF0HSBFLws4n5UPyd)

1. Intermediate event node
2. Intermediate event

updating\\

1. Message Intermediate Catch Event

#### Config:

1. Message Intermediate Throw Event

#### Config:

1. Timer Intermediate Catch Event

Flow runs when this node catches the start timer. Like the Timer start event, this node allows to config start time as a condition for flow to go through this node to the next task or run task which contains this event

#### Config:

* Time cycle (cron) : Specifies repeating intervals
* Time date in ISO-8601 : Set start time at a point in time
* Time duration: To specify how long the timer should run before it is fired

![](https://lh6.googleusercontent.com/8VB8mffsly6nF8wWZEpQwezkZgluae5-jMZxyrpsT8YoMa5NSQE4qIka81MBsMKWD5gZnI98OovQajZau98dN3joTMZwAxiQAGYyvFcakLemNHnaUDfoUaCKj5VlSVP7TNh7YkPN)

1. Escalation Intermediate Throw Event

Escalating to a higher level of responsibility.

#### Config:

1. Conditional Intermediate Catch Event

#### Config:

1. Link Intermediate Throw Event

#### Config::

1. Link Intermediate Throw Event

#### Config:

1. Compensation Intermediate Catch Event

Reivece signal from Compensation Intermediate Throw Event and active compensation task. This node is stuck on the task where there is a branch to compensation task

1. Compensation Intermediate Throw Event

Throw a signal to all comensation event in the instance workflow

#### Config:

1. Signal Intermediate Catch Event

Running to this node, the flow status will change to “waiting”. In order to pass this node or run a task containing this node, flow needs to catch a signal from the throw signal event.

#### Config:

* Signal reference : Select Signal name (Need declare signal definition on general right sidebar)

![](https://lh4.googleusercontent.com/b0\_yDcI532pjjDMld7lMKK9KoS86s0Vc1VE9X-gAcXlYuHiv8LJdqdpZihxiYQZ8NBpOwq473LiL\_1W4LTDQyVRb0rQ3UxztVQKpirXrVU3YJ-wd9tB7Mwvg7q4lNgOmIoWLIuOz)

1. Signal Intermediate Throw Event

This node throws spread a signal and flow still continues to the next node

#### Config:

* Signal reference: Select Signal name (Need declare signal definition on general right sidebar)

![](https://lh3.googleusercontent.com/fhiwqDZV-3BerWZEzq55s4Ol0NYNIL8cxFD4a6UYp7dTa24n4LIDMIomWpqq17ybKtACDw\_isRnyIVYp7MOL0e-TnyWkGruz2CjWvkK1LQJBUKV0KIHU\_dQYYhy6pmGT59wnq-jT)

* Declare signal definitions:
* ID: id signal

Signal could be caught by same id signal \\

* Name: name of signal

This name will be show in drop list of signal reference

* Scope:

![](https://lh3.googleusercontent.com/O6NezSFM5ihtIIuUapUbcf9FIY8u23D9xCFa4BhqEDEyuAog4PPFx4dvmpEaUgsc4OT65Oa9GbclI\_PG-f9i2WEhSBFhjYpUom2wEVakVFwMSTu8wrGtd1GnXGpvkx8zhdneP\_Vr)

1. End event node (The last node to close/end process)
2. End Event

end process instance

1. Message End Event

updating\\

1. Escalation End Event

updating\\

1. Error End Event

updating\\

1. Compensation End Event

updating\\

1. Signal End Event

End process instance and throw signal\\

1. Terminate End Event

To stop process instance immediately

#### Config:

* Terminate all: Stop all the same process instance
