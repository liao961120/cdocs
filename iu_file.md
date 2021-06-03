IU 時間檔
================

上傳語料檔時，若出現重新切分 IU 或新語料檔 (且有錄音檔) 時，需額外提供 **IU 時間檔**，以重新切割錄音檔，用於網站上的 IU 以及句子的發音。請助理準備**三份檔案**繳交給我：


## 語料檔

- 檔案名稱形式：`<corpus_filename>.txt`  
    - `<corpus_filename>` 僅能使用英文字母、數字以及 `-` 與 `_` (不可出現空白)
    - 範例：[`skzyNr-pear_panay.txt`][corpFile]
- 內容格式：見[語料檔格式](corpus_file)


## 錄音檔

!> 錄音檔請使用 `.mp3` 格式，並且**只能有一個**。若有多個，請在切分 IU 之前將多個錄音檔合併成一個，再以此錄音檔為準進行切分。

- 檔案名稱形式：`<corpus_filename>.mp3`
    - 此檔名必須同時出現在語料檔 meta data 的 **`video`** 之中
    - 範例：[`skzyNr-pear_panay.mp3`][audioFile]


## IU 時間檔

- 檔案名稱形式：`<corpus_filename>IU.txt`
    - 範例：[`skzyNr-pear_panayIU.txt`][iuFile]
- 內容格式 (由 Praat 輸出轉換而來，詳情請問宋老師)：
    ```
    1 0.36 1.63
    2 2.92
    3 3.50
    ...
    42 119.99
    43 123.11
    44 126.43
    ```


[corpFile]: https://github.com/liao961120/cdocs/blob/main/_media/examples/skzyNr-pear_panay.txt
[audioFile]: https://github.com/liao961120/cdocs/blob/main/_media/examples/skzyNr-pear_panay.mp3
[iuFile]: https://github.com/liao961120/cdocs/blob/main/_media/examples/skzyNr-pear_panayIU.txt
