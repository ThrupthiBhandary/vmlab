# VirtualBox – Linux Installation and C Program Execution

## Program 1: Install VirtualBox and Linux/Windows Operating System

### Aim

To install **Oracle VirtualBox** and set up a Linux or Windows operating system as a virtual machine on a Windows host system.

### Requirements

- Windows 7/8/10/11 host system
- Oracle VirtualBox
- Linux/Windows ISO or `.ova` virtual appliance file
- Sufficient RAM and storage

### Procedure

#### Step 1: Download VirtualBox

1. Download the **VirtualBox installer (`.exe`)**.
2. Open the downloaded `.exe` file.
3. The VirtualBox Setup Wizard will appear.
4. Click **Next**.

#### Step 2: Choose Installation Options

1. Review the installation location and components.
2. Click **Next**.

#### Step 3: Create Shortcuts

1. Select the required shortcut options.
2. Click **Next**.

#### Step 4: Network Interface Warning

1. A warning about network interfaces may appear.
2. Click **Yes** to continue.

#### Step 5: Install VirtualBox

1. Click **Install**.
2. Wait for the installation to complete.

#### Step 6: Complete Installation

1. Once the installation is completed, click **Finish**.
2. The **VirtualBox** application will be available from the Desktop or Start Menu.

---

## Program 2: Install a C Compiler and Execute a Simple C Program

### Aim

To install and use a **C compiler** in a Linux virtual machine created using VirtualBox and execute a simple C program.

### Procedure

## Part A: Import Ubuntu Virtual Machine

1. Open **Oracle VirtualBox**.
2. Select **File → Import Appliance**.
3. Click **Browse**.
4. Select the Ubuntu virtual appliance file:

```text
ubuntu_gt6.ova
```

5. Select the imported Ubuntu virtual machine.
6. Go to **Settings**.
7. Select **USB**.
8. Configure the USB controller as required, such as **USB 1.1**.
9. Click **Start** to launch the Ubuntu virtual machine.

---

## Part B: Run a C Program

### Step 1: Open Terminal

Open the **Terminal** in the Ubuntu virtual machine.

### Step 2: Navigate to the Required Directory

Execute:

```bash
cd /opt/axis2/axis2-1.7.3/bin
```

### Step 3: Create the C Program

Create a C source file using:

```bash
gedit hello.c
```

Enter the following simple C program:

```c
#include <stdio.h>

int main()
{
    printf("Hello World!\n");
    return 0;
}
```

Save the file and close the editor.

### Step 4: Compile the Program

Compile the C program using:

```bash
gcc hello.c
```

If there are no compilation errors, an executable file named `a.out` will be created.

### Step 5: Execute the Program

Run the compiled program:

```bash
./a.out
```

### Step 6: Display the Output

The output will be:

```text
Hello World!
```

---

## Result

1. VirtualBox was successfully installed on the Windows host system.
2. Ubuntu was successfully imported and executed as a virtual machine.
3. The GCC C compiler was used to compile the C program.
4. The C program was successfully executed and the output was displayed.

## Conclusion

VirtualBox was successfully installed and used to run a Linux virtual machine. A C compiler was used inside the virtual machine to compile and execute a simple C program successfully.
