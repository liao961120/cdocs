錄音資訊更新
================

上傳語料檔時，若出現重新切分 IU 或有新語料檔 (且有錄音檔) 時，需額外提供 **IU 時間檔**，以重新切割錄音檔，用於網站上的 IU 以及句子的發音。請助理準備**三份檔案**繳交給我：


## 語料檔

- 檔案名稱形式：`<corpus_filename>.txt`  
    - `<corpus_filename>` 僅能使用英文字母、數字以及 `-` 與 `_` (不可出現空白)
    - 範例：[`skzyNr-pear_panay.txt`][corpFile]
- 內容格式：見[語料檔格式](corpus_file)


## 錄音檔

!> 錄音檔請使用 `.mp3` 格式，並且**只能有一個**。若有多個，請先將多個錄音檔合併成一個，再以此音檔為準做為 IU 切分時間資訊的依據。

- 檔案名稱形式：`<corpus_filename>.mp3`
    - 此檔名必須同時在語料檔的 `video` 進行定義。範例見 `skzyNr-pear_panay.txt` 的[第七行](https://github.com/liao961120/cdocs/blob/a936c8292721726b9345d316fcf00dfd2587ff47/_media/examples/skzyNr-pear_panay.txt#L7)：
    ```
    topic: pear_panay
    type: Narrative
    language: 撒奇萊雅語, Sakizaya, Sakizaya
    speaker: 葉阿妹, panay, female, 1949-11-20
    collected: 2008-01-05
    revised: None
    video: skzyNr-pear_panay.mp3
    ```
    - 範例：[`skzyNr-pear_panay.mp3`][audioFile]


## IU 時間檔

- 檔案名稱形式：`<corpus_filename>IU.txt`
    - 範例：[`skzyNr-pear_panayIU.txt`][iuFile]
- 內容格式 (由 Praat 輸出轉換而來，詳情請詢問宋老師)：
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
