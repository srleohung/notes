# 060E1-Acquisition

## 1. Why it is necessary to create a duplication of the original media during the forensic investigation process?

<details>
<summary>Answer</summary>
<p>
Digital evidence are highly fragile, analyzing the original evidence could easily altered, damaged or even destroyed the evidence.

To prevent accidental or intentional manipulation of the original evidence, it is necessary to create a duplication of the original media during the forensic investigation process. The resulted forensic image is identical in every way to the original, not only including the working files, but also hidden, erased, fragmented, corrupted, temporary and special attribute files.
This allows storing the original media away, safe from harm while the investigation proceeds using the disk image.
<details>
<summary>Translate</summary>
<p>
數字證據是非常脆弱的, 分析原始證據可以輕易塗改, 損壞甚至摧毀了證據。

為了防止原始證據的意外或故意操縱, 有必要在法庭調查過程中創建原始媒體的複製。所得法醫圖像中的每個日日夜夜原來的, 不僅包括工作文件相同, 但也隱藏, 刪除, 碎片, 損壞, 臨時的和特殊的屬性文件。這使得在使用磁盤鏡像調查所得不受傷害存儲原始媒體了, 是安全的。
</p>
</details>  
</p>
</details>  

## 2. Assume that you received an external portable hard drive from the evidence collection team of your company, and you are assigned to create a copy of the hard drive.
### (a) Name a software that can be used to image the data in the hard drive.

<details>
<summary>Answer</summary>
<p>
AccessData FTK Imager.
Several tools are available to image data, such as AccessData FTK Imager, EnCase Forensic Imager, and the utility dd in Unix/Linux.
<details>
<summary>Translate</summary>
<p>
AccessData FTK Imager。

幾個工具可用來的圖像數據, 諸如的AccessData FTK成像儀, 包住法醫成像儀, 和在Unix / Linux中的利用dd。
</p>
</details>  
</p>
</details>  

### (b) You are going to use the software you mentioned in (a) for creating the copy. Write down the steps, including the hardware and/or software you will use, for performing the task.

<details>
<summary>Answer</summary>
<p>

1. Connect the portable hard drive to a hardware-based write blocker.
2. Connect the hardware-based write blocker to the computer.
3. Start FTK Imager to create a forensic image of the hard drive.
4. Check the output of FTK Imager to ensure the resulted forensic image is exactly the same as the original source.
5. Start a software-based write blocker application on the computer, and start the write-blocking function.
6. Connect the portable hard drive to the computer.
7. Start FTK Imager to create a forensic image of the hard drive.
8. Check the output of FTK Imager to ensure the resulted forensic image is exactly the same as the original source.
<details>
<summary>Translate</summary>
<p>

1. 連接的便攜式硬盤驅動器, 以基於硬件的寫阻斷劑。
2. 連接的基於硬件的寫阻滯劑到計算機。
3. 開始FTK成像以創建硬盤驅動器的法醫圖像。
4. 檢查FTK成像儀的輸出, 以確保所得到的法醫圖像是完全一樣的原始源。
5. 在計算機上啟動的基於軟件的寫入攔截應用, 並啟動阻塞寫功能。
6. 連接的便攜式硬盤驅動器和計算機。
7. 開始FTK成像以創建硬盤驅動器的法醫圖像。
8. 檢查FTK成像儀的輸出, 以確保所得到的法醫圖像是完全一樣的原始源。
</p>
</details>  
</p>
</details>  

### (c) How can you verify that during the process of media duplication, the original media is unchanged?

<details>
<summary>Answer</summary>
<p>
It is necessary to generate hash reports of the original media, which is used as a benchmark to prove the integrity of the evidence. Algorithms such as Secure Hash

Algorithm (SHA-1) and SHA-2, or Message Digest 5 (MD5) can be used as the hash function.
When the portable hard drive is imaged, a drive hash and an image hash are generated for verification. The drive hash should match the hash reports of the original media to prove that the original media is unchanged during the process of media duplication.
<details>
<summary>Translate</summary>
<p>
有必要產生原始媒體, 它被用來作為基準來證明證據的完整性的散列報告。算法, 例如安全散列算法（SHA-1）和SHA-2, 或消息摘要5（MD5）可以用作散列函數。

當便攜式硬盤驅動器進行成像時, 針對驗證生成的驅動散列和圖像散列。驅動散列應匹配原始媒體的哈希報告, 證明原來的媒體是重複的過程中保持不變。
</p>
</details>  
</p>
</details>  