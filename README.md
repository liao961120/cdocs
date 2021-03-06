{docsify-updated}

南島語料庫管理說明
=================



## 網站更新流程


[Open PDF](_media/data_update_flow.pdf ':target=_blank :ignore')

<embed src="_media/data_update_flow.pdf#view=FitH&scrollbar=1&toolbar=0&navpanes=0" width="100%" height="520" type="application/pdf" class="pc">

<img src="_media/data_update_flow.png" width="100%" class="mobile">


## 重要連結

### 內文

1. [語料檔格式][textFormat]
2. [錄音資訊更新][timeFormat]

### 外部

1. [Google Drive][GD] (for 網站)
2. [啟動資料更新][corpUpdate]
3. [語料統計資訊][corpStats]


[GD]: https://drive.google.com/drive/folders/157b3nuLmqqZZrXzw0MOas_l3s6MWnK7Q
[corpUpdate]: https://cdocs.netlify.app
[textFormat]: corpus_file
[timeFormat]: iu_file
[corpStats]: https://yongfu.name/glossParser/meta/



## 網站 Google Drive 結構

```tree
.
├── 網頁資訊
│   ├── about.md
│   ├── about-en.md
│   ├── external_links.md
│   ├── external_links-en.md
└── 公開語料
    ├── sentence
    │   ├── Bunun_Isbukun
    │   |   ├── 1.txt
    │   |   └── 2.txt
    │   └── Kanakanavu_Kanakanavu
    │       ├── 1.txt
    │       └── ...
    └── story
        ├── Amis_Ciwkangan
        |   ├── Amis_Conv-farming_marang_furayang.txt
        |   ├── Amis_Nr-frog_cinhua.txt
        |   └── ...
        ├── Atayal_Mayrinax
            ├── AtaNr-dailylife1_Iwan.txt
            └── ...
        ├── Rukai_Vedai
        ├── ...
        └── Tsou_Tfya
```