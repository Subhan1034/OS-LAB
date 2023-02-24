# TASK 1: Manual of Installation of VMware Workstation 17 Player and Ubuntu

---

> In this lab, the following software will be installed:
>
> * VMware Workstation 17 Player
>
>
> * Ubuntu`

##VMware Workstation 17 Player

**Step 1:** Click on the click [VMware Workstation 17 Player]([VMware Workstation Player - VMware Customer Connect](https://customerconnect.vmware.com/en/downloads/details?downloadGroup=WKST-PLAYER-1700&productId=1377&rPId=97014)) 

**OR**

In case the link does not work you can follow the steps listed below:

1. Click on *"Search bar"* in "Browser" and type **VM player 17** and hit *Enter* as shown in figure below:

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\I.png)

2. Click on *"VMware Workstation Player"* as illustrated below :

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\II.png)

3. The website of **vm**ware will be opened click on *Download free*:

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\III.png)

4. Click on *"Go to Downloads"*  as shown in figure below:

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\IIII.png)





**Step 2: ** Install exe according to your OS(Linux or Windows) by clicking on **"Download Now"**:

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\V.png)



**Step 3: ** Run exe file and click on Yes to  **"Install VM Workstation Player"**:

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\Vi.png)



**Step 4: ** Click on Next Accept the License  and change directory (if you want not recommended):

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\VIi.png)



**Step 5:** Click on Finish and you are done installing **VMware Workstation 17 Player**.

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\VIiI.png)

---



## Ubuntu

**Step 1:** Download the iso file from **Ubuntu** website by clicking on the link [Download Ubuntu Desktop](https://ubuntu.com/download/desktop).
Note:*You should download* **Ubuntu 22.04.1 LTS**.

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\IX.png)

**Step 2:** Open **VMware Workstation 17 Player** installed before.



![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\X.png)

**Step 3 :** Click on **Create a New Virtual Machine** as illustrated below.

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\XI.png)

**Step 4 :** Check Mark **I will install Operating System later** and Click on *Next* button.

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\XII.png)

**Step 5 :** Check Mark **I will install Operating System later** and Click on *Next* button.

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\XIII.png)

**Step 6 :**  Click on *Next* button *(If you want to change storage location you can but it is not recommended)*.

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\XIV.png)

**Step 7 :** Click on *Next* button *(If you want to change storage Size)*.

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\XV.png)

**Step 8 :** Click on *Customize Hardware* button.

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\XVI.png)

**Step 9 :** Click on *Memory* and slide the bar to  **at least 4GB ** and Click on *New CD/DVO (SATA)*, check mark *use ISO image file* and Browse to *file location of ISO File* then click on **Close**.

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\XVII.png)

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\XX.png)

**Step 10 :** Click on *finish*.

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\XVIII.png)

**Step 11 :** Click on *Ubuntu 64-bit*.

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\XXII.png)

**Step 12 :** Click on *Play Virtual Machine*.

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\XXIII.png)



**Step 13 :** A black screen will appear *(will take some time depending on Internet Speed)*.

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\XXIV.png)

**Step 14 :** Change language and set password according to you preferences.

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\a.png)





**Step 15 :**A black screen will appear with a progress bar *(will take some time depending on Internet Speed)* .

![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\XXVI.png)



**Step 16 :** Congratulations! After a rigorous journey of following steps we are done setting up environment for **Linux**.



![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\XXV.png)



# TASK 2: Test the gcc and g++ compilers installation of your installed Ubuntu OS.

------

> **Ctrl + Alt + T** is shortcut key to open Terminal

1.  Open Terminal using **Ctrl+Alt+T**

2. Type *g++ -v* to check g++ version and hit enter. If error message saying **command not found** then use *sudo apt install g++* to install **g++**

   ![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\2I.png)

3. Type **touch** *testFile.cpp* to make a cpp file.

   ![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\2II.png)

4. Type **ls**  to view list and verify.

   ![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\2II.png)

5. Type **nano** *testFile.cpp* to open in editor to write code. Alternatively you cane use **gedit** *testFile.cpp* to open edit cpp file in gedit.

   ![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\2IV.png)

6. Type sample code cat testFtIe. cpp

   ```c++
   #include <iostream>
   using namespace std;
   int main()
   {
     	cout<<"I love coding " ;
   	return 0;
   }

   ```

   ![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\2III.png)

7. Type **g++ testFile.cpp -o testFile.exe** and hit enter use *ls* to verify exe creation.
   ![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\2IV.png)

8. Use *./testfile.exe*

   ![Image illustrating user Clicking on *"Search bar"* in "Browser" and typing **VM player 17**](\2V.png)