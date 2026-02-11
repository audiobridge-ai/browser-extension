# Windows Installation Guide (Unsigned Installer)

Because this app is distributed **without a Microsoft code-signing certificate**, Windows may display a security warning during installation.
This is normal behavior for independent software and **does not indicate malware**.

Please follow the steps below to install successfully.

---

## Method 1 (Most Common)

### “More info” → “Run anyway” (Windows SmartScreen)

This is the standard and recommended way.

### Steps

1. Double-click the installer
   Example:

   ```
   YourAppSetup.exe
   ```

2. Windows will show a blue warning screen:

   > **“Windows protected your PC”**
   > Microsoft Defender SmartScreen prevented an unrecognized app from starting.

3. Click **“More info”**

4. Click **“Run anyway”**

5. The installer will start normally
   Follow the on-screen instructions to complete installation

✅ After this, Windows usually remembers your choice and will not block it again.

---

## Method 2 (If Windows Defender blocks the file)

### Allow the installer in Windows Security

Use this if the file was **blocked or removed after download**.

### Steps

1. Open **Windows Security**

   * Start Menu → search **“Windows Security”**

2. Go to:

   ```
   Virus & threat protection
   ```

3. Click **Protection history**

4. Find the entry related to your installer

5. Click it, then choose:

   * **Allow on device**
     or
   * **Restore**

6. Run the installer again

---

## One-line explanation for users

> If Windows shows “Windows protected your PC”, click **More info** and then **Run anyway**. This is a normal Windows security check for unsigned apps.
