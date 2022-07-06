### Một số command line phổ biến POWERSHELL

1.  Hiện đường dẫn làm việc hiện tại:

    Print Working Directory `pwd`, Get-Location `gl`

    ```bash
    > pwd
    > D:\Workspace
    ```

2.  Hiện các file trong thư mục hiện tại:

    List `ls`, Get-ChildItem `gci`, directory `dir`

    ```bash
    > ls
    > src app README.md
    ```

3.  Chuyển vị trí làm việc:

    Change the directory `cd`, `chdir` Set-Location `sl`

    Chuyển dến đường dẫn x `cd x`

    ```bash
    > ls
    > Directory: D:\Workspace\src
    > cd x
    > Directory: D:\Workspace\src\x
    ```

    Chuyển vị trí trước đó `cd -`

    ```bash
    > cd -
    > Directory: D:\Workspace\src
    ```

    Chuyển vị trí ra bên ngoài `cd ..`

    ```bash
    > cd ..
    > Directory: D:\Workspace
    ```

4.  Làm việc với file và folder

    Tạo folder: make directory `mkdir`

    ```bash
    > mkdir newFolder
    ```

    Tạo file: New-Item `ni`

    ```bash
    > ni newFile.txt
    ```

    Sao chép file: Copy-Item `Copy-Item`, copy `cp`

    ```bash
    > cp newFile.txt newFile2.txt
    ```

    Di chuyển file: move `mv`

    ```bash
    > mv newFile.txt newFolder
    ```

    Đổi tên file: Rename-Item `Rename-Item`, move `mv`

    ```bash
    > mv newFile.txt newNewFile.txt
    > Rename-Item newNewFile.txt superNewFile.txt
    ```

    Xóa file, xóa folder: remove `rm`

    ```bash
    > rm newNewFile.txt
    > rm newFolder
    ```

5.  Hiện text file, cat `cat`

    ```bash
    > cat helloWorld.txt
    > hello world
    ```

    `cat` có thể hiện nhiều file

    ```bash
    > cat helloWorld.txt helloWorld2.txt
    > hello world hello world2
    ```

    `cat` có thể hiện nhóm file, dấu `>` tạo file nhóm

    ```bash
    > cat helloWorld.txt helloWorld2.txt > helloWorld3.txt
    > cat helloWorld3.txt
    > hello world hello world2
    ```

6.  Hiển thị với `echo`

    ```bash
    > echo hello every one
    > hello every one
    ```

    `echo` còn có thể ghi đè và file với `>`

    ```bash
    > echo hi > .\README.md
    > cat .\README.md
    > hi
    ```

    `echo` có thể ghi vào cuối file với `>>`

    ```bash
    > echo xin chao >> .\README.md
    > cat .\README.md
    > hi xin chao
    ```
