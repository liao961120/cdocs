語料檔
============

## 內容結構

每份語料檔的內部可以分成兩種類別：「語料資訊」與「IU」。語料資訊是記載這份語料收錄時的資訊，例如日期、語言、發音人等等；IU 則是收錄到的語言轉寫與分析。

```
[語料資訊]

[IU 1]

[IU 2]

[IU 3]

...
```

## 語料資訊

每份語料檔的一開頭 (不可以有空行) 為語料資訊區塊。長相如下：

```
topic: pear_panay
type: Narrative
language: 撒奇萊雅語, Sakizaya, Sakizaya
speaker: 葉阿妹, panay, female, 1949-11-20
collected: 2008-01-05
revised: None
video: skzyNr-pear_panay.mp3
```

- 上方的每行都是一項資訊，結構以 `<資訊種類>: <內容>` 書寫。注意，請使用**半形**冒號 `:`，冒號之後需加上一個**半形空白**
- 這些資訊之中，`language`、`speaker`、`collected` 是必要的；如果有相對應的音檔，請寫在 `video`；`topic` 與 `type` 則是篇章類型的語料才需提供。在寫下這些資訊時，請檢查是否**拼錯**，並且全部使用**小寫**

!> 寫完語料資訊之後，**務必要留一行以上的空行**後再開始下個部份 (語言轉寫)。


## 語言轉寫與分析格式

下方為 **1 個句子或 IU** 的轉寫範例，支援兩種格式：

1. **三行** gloss lines (切分且對齊之*族語*、*英文*、*中文*)；**三行** free lines (中英翻譯及註釋)

    ```
    [編號].
    [族語分析 (aligned)]
    [英文 Glossing (aligned)]
    [中文 Glossing (aligned)]
    [空行]
    #e [英文翻譯]
    #c [中文翻譯]
    #n [註釋]
    [空行]
    ```

	<details>
	<summary>(範例語料)</summary>

	```
	2.
	si-pa-quwas=mu           i      yaya
	CF-VBL-song=1SG.GEN      NOM    mother
	參焦-動化-歌=1SG.屬格      名詞    媽媽
	
	#e I sing for mom.
	#c 我唱歌給媽媽聽。
	#n i 可以省略。
	```

	</details>


2. **一行**原始族語 (未切分)；**三行** gloss lines (切分且對齊之*族語*、*英文*、*中文*)；**三行** free lines (中英翻譯及註釋)

    ```
    [編號].
    [族語轉寫 (原始)]
    [空行 (optional)]
    [族語分析 (aligned)]
    [英文 Glossing (aligned)]
    [中文 Glossing (aligned)]
    [空行]
    #e [英文翻譯]
    #c [中文翻譯]
    #n [註釋]
    [空行]
    ```

	<details>
	<summary>(範例語料)</summary>

	```
	2.
	sipaquwasmu i yaya

	si-pa-quwas=mu           i      yaya
	CF-VBL-song=1SG.GEN      NOM    mother
	參焦-動化-歌=1SG.屬格      名詞    媽媽
	
	#e I sing for mom.
	#c 我唱歌給媽媽聽。
	#n i 可以省略。
    ```

	</details>

!> `[編號].`：編號後的 **`.`** 是**必須**的，且 `[編號].` 需獨占一行


## 注意

!> Gloss lines 的每個單位**皆**要有內容，若暫時不確定如何分析，請使用**底線** (`_`) 替代：

<details>
<summary>(範例語料)</summary>

```
si-pa-quwas=mu     i     yaya
CF-VBL-song=_      NOM   mother
參焦-動化-歌=_      名詞   媽媽
```

</details>



!>  Gloss lines 中的**同一個切分單位**之內**不可以有空白**。若有多重意義，請使用 dot (`.`) 當作連接符號，例如下方的 `good.beautiful`, `好.漂亮`：

<details>
<summary>(範例語料)</summary>

```
mathariri       kay     akaneane
good.beautiful  this    food
好.漂亮          這      食物
```

</details>


!> 若 gloss lines **一行寫不下**，請依循下方格式換行  
   其它行，例如第一行未切分的**原始族語**與 **free lines** 請**勿換行**書寫。

<details>
<summary>(範例語料)</summary>

```
[族語分析]
[英文 Glossing]
[中文 Glossing]
[空行 (Optional)]
[族語分析 (接續，第二行)]
[英文 Glossing (接續，第二行)]
[中文 Glossing (接續，第二行)]
[空行 (Optional)]
[族語分析 (接續，第三行，如果還有)]
[英文 Glossing (接續，第三行，如果還有)]
[中文 Glossing (接續，第三行，如果還有)]

15.
kay lasitu nguavavaeva mucucubungu kilrumay ki sinsilini

kay   la-situ       ngu-a-va-vaeva   mu-cucubungu  ki-lrumay
this  PL-student    ngu-RLS-RED-one  go-front      PASS-hit
這    複數-學生       ngu-實現-重疊-一  去-前面        被-打

ki   sinsi-lini
OBL  teacher-3PL.GEN
斜格  老師-他們的

#e The students went to the front one by one to be hit by their teacher.
#c 這些學生一個個到前面被他們的老師打
```

</details>


## 檔案格式

- 檔案類型  
支援的檔案格式為純文字檔 (`.txt`)，請使用 UTF-8 編碼。
