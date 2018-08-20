Data and Control Functions
---------------------------

20 ARGET
~~~~~~~~

query
^^^^^

Datafiled
    1 - 資料型態 - 1 byte

    2 - 資料長度 - 2 bytes

Response
^^^^^^^^
IF OK
    1 ACK + 1 DATA

Datafiled
    1 - 資料型態 - 1 byte

    2 - 資料長度 - 2 bytes

    3 - 資料     - N bytes

IF NO OK
    1 NACK

21 ARPUT
~~~~~~~~

query
^^^^^

Data 3 bytes

1 - 資料型態 - 1 byte

2 - 資料長度 - 2 bytes

3 - 資料     - N bytes

Response
^^^^^^^^
IF OK
1 ACK

IF NO OK
1 NACK

22 STGET
~~~~~~~~

query
^^^^^

Datafiled
    1 - 資料型態 - 1 byte

    2 - 資料長度 - 2 bytes

Response
^^^^^^^^
IF OK
    1 ACK + 1 DATA

Datafiled
    1 - 資料型態 - 1 byte

    2 - 資料大小 - 2 bytes

    3 - 資料     - N bytes

IF NO OK
    1 NACK

23 STPUT
~~~~~~~~

query
^^^^^

Datafiled
    1 - 資料格式字串長度 - 1 byte

    2 - 資料格式字串 - N bytes

    3 - 資料大小 - 2 bytes

    4 - 資料 - M bytes

Response
^^^^^^^^
IF OK
    1 ACK

IF NO OK
    1 NACK
