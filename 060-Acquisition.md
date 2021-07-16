# 060-Acquisition

## Evidence acquisition 取證

* Analysing the original evidence could modify or even destroy the evidence
* Necessary to acquire the original digital evidence in a manner that `protects and preserves` the evidence
<details>
<summary>Translate</summary>
<p>

* 分析原始證據可能會修改甚至破壞證據
* 必須以`保護和保存`證據的方式獲取原始數字證據
</p>
</details>  

## Types of acquisition 採集類型

* Live data acquisition 實時數據採集
  + Acquisition of volatile data (live forensics) 獲取易失性數據（實時取證）
* Static data acquisition 靜態數據採集
  + Acquisition of non-volatile data 獲取非易失性數據

## Live forensics 現場取證

* System information 系統信息
* Current configuration and running state of computer 電腦當前配置和運行狀態
* Volatile system information 易失的系統信息
* Network information 網絡信息

## Static data acquisition 靜態數據採集

* Non-volatile information 非易失性信息
* Files / data in storage media 存儲介質中的文件/數據
* Data includes slack space, swap files, unallocated drive spaces 數據包括空閒空間、交換文件、未分配的驅動器空間

## The need of media duplication 媒體複製的必要性

* Disk or media duplication is at the core of computer forensics process
* Necessary to create an `exact` copy of the original disk/ media for analysis because of the volatility of the data on the disk and potential that evidence could be modified or destroyed during handling and analysis
<details>
<summary>Translate</summary>
<p>

* 磁盤或媒體複製是計算機取證過程的核心
* 必須創建原始磁盤/媒體的`精確`副本以供分析, 因為磁盤上數據的易失性以及在處理和分析過程中證據可能被修改或破壞的可能性
</p>
</details>  

## Simple backup / copy...

* Only copied the active data
  + i.e., All the files you can see
  + Not include slack, residue, deleted files
  + May not capture the timestamp of the data
<details>
<summary>Translate</summary>
<p>

* 只複製活動數據
   * 即, 您可以看到的所有文件
   * 不包括鬆弛、殘留、刪除的文件
   * 可能無法捕獲數據的時間戳
</p>
</details> 

## Bit stream image

* To be complete and accurate, the copy should be a `bit-by-bit clone` of the original disk, called a `bit stream image`
* A bit stream copy is recording every single bit (0 or 1) of data that resides on a storage device
* The bit stream copy allows copying of working files, and also `hidden, erased, fragmented, corrupted, temporary and special attribute files`
<details>
<summary>Translate</summary>
<p>

* 為了完整和準確, 副本應該是原始磁盤的`逐位克隆`, 稱為`位流圖像`
* 位流副本記錄駐留在存儲設備上的數據的每一位（0 或 1）
* 比特流複製允許複製工作文件, 也允許複製`隱藏、擦除、碎片化、損壞、臨時和特殊屬性文件`
</p>
</details> 

## Preparation of the media 媒體的準備

* A brand new media / clean media
* Media sanitisation
  + Clear
    - Logical techniques using standard read-write commands
  + Purge
    - Physical / logical techniques to make target data recovery infeasible by state-of- the-art laboratory techniques
  + Destroy
    - Use of state-of-the-art laboratory techniques but result in inability to use the media for data storage (e.g., cross-cut shredding)
<details>
<summary>Translate</summary>
<p>

* 全新的媒體/乾淨的媒體
* 媒體消毒
   * 清除

     - 使用標準讀寫命令的邏輯技術

   * 清除

     - 通過最先進的實驗室技術使目標數據恢復不可行的物理/邏輯技術

   * 破壞

     - 使用最先進的實驗室技術, 但導致無法使用介質進行數據存儲（例如, 橫切切碎）

</p>
</details> 

## Write protection 寫保護

* Write protection should be initiated to preserve and protect the original evidence
* A `write blocker` is any tool that permits `read-only` access to data storage devices without compromising the `integrity` of the data
* Two types of write blockers:
  + Hardware write blockers
  + Software write blockers
<details>
<summary>Translate</summary>
<p>

* 應啟動寫保護以保存和保護原始證據
* `寫阻止程序`是允許對數據存儲設備進行`只讀`訪問而不損害數據`完整性`的任何工具
* 兩種寫攔截器：
   * 硬件寫攔截器
   * 軟件寫攔截器 
</p>
</details> 

## Disk imaging 磁盤映像

* Disk imaging can be done using software
  + Forensics application suite
    - Examples: EnCase® Forensic, AccessData® FTK®
  + Forensics imaging utility
    - Examples: EnCase® Forensic Imager, AccessData® FTK® Imager, dd
<details>
<summary>Translate</summary>
<p>

* 磁盤映像可以使用軟件完成
   * 取證應用套件

     - 示例：EnCase® Forensic, AccessData® FTK®

   * 取證成像實用程序

     - 示例：EnCase® Forensic Imager, AccessData® FTK® Imager, dd

</p>
</details> 

## AccessData® FTK® Imager

* A data preview and imaging tool that allows quickly assess of digital evidence
* Allows creating forensic sound images of different media
  + Makes a bit-by-bit duplicate of the media
* The forensic image is identical in every way to the original, including file slack and unallocated space or drive free space
<details>
<summary>Translate</summary>
<p>

* 一種數據預覽和成像工具, 可以快速評估數字證據
* 允許創建不同媒體的法醫聲像
   * 逐位複制媒體
* 取證圖像在各方面都與原始圖像相同, 包括文件鬆弛和未分配空間或驅動器可用空間
</p>
</details> 

## Integrity of disk copy 磁盤拷貝完整性

* Have to prove that the disk image is `exactly` the same as the original evidence
* Comparison of a digital fingerprint
* `Hashes` of the original evidence and disk image should be created
<details>
<summary>Translate</summary>
<p>

* 必須證明磁盤映像與原始證據`完全`相同
* 數字指紋的比較
* 應創建原始證據和磁盤映像的`哈希值`
</p>
</details> 

## Hashing 散列

* Hashing is a mathematical process (via an algorithm) that produces a unique value (hash value) that is essentially the digital "fringerprint" or "DNA" of a particular file, piece of media, etc
* This digital fingerprint can be used to compare the original evidence to the forensic image
  + These two values should match exactly
<details>
<summary>Translate</summary>
<p>

* 散列是一個數學過程（通過算法）, 它產生一個獨特的值（散列值）, 它本質上是特定文件、媒體等的數字“邊緣印記”或“DNA”
* 此數字指紋可用於將原始證據與法醫圖像進行比較
   * 這兩個值應該完全匹配
</p>
</details> 

## Types of hashing algorithm 哈希算法的類型

* Common hash functions 常用哈希函數: 
  + Message Digest 5 (MD5)
  + Secure Hash Algorithm (SHA-1) and SHA-2

## Use of hashing 散列的使用

* Hash values can be used throughout the digital forensic process
  + Used after the cloning process to verify that the clone is indeed an `exact duplicate`
  + Used as `an integrity check` at any point
  + Used to `identify` specific files
* Recorded throughout the chain of custody
<details>
<summary>Translate</summary>
<p>

* 哈希值可用於整個數字取證過程
   * 在克隆過程之後用於驗證克隆確實是 `完全重複` 的
   * 在任何時候用作 `完整性檢查`

   * 用於 `識別` 特定文件
* 在整個監管鏈中記錄
</p>
</details> 
