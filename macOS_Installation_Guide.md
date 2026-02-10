# macOS Installation Guide (Unsigned PKG)

Because this app is distributed as an **unsigned `.pkg` installer** (not notarized by Apple), macOS Gatekeeper may block it on first install.
This is expected behavior on macOS and **does not mean the app is unsafe**.

Please follow the steps below to complete installation.

---

## Method 1 (Recommended)

### Right-click → Open the PKG installer

This is the **simplest and Apple-recommended way**.

### Steps

1. Locate the downloaded installer
   Example:

   ```
   YourAppInstaller.pkg
   ```

2. **Right-click** the `.pkg` file
   (or hold **Control** and click)

3. Select **“Open”**

4. A security dialog will appear saying the developer cannot be verified
   Click **“Open”** to confirm

5. The installer will launch normally
   Follow the on-screen steps to finish installation

✅ After this, the installer will not be blocked again.

---

## Method 2 (If the installer was already blocked)

### System Settings → Privacy & Security → Open Anyway

Use this if the user **double-clicked the PKG and it failed**.

### Steps

1. Double-click the `.pkg` installer
   macOS shows:

   > “This package can’t be opened because it is from an unidentified developer.”

2. Open:

   ```
   System Settings → Privacy & Security
   ```

3. Scroll down to the **Security** section

4. You will see a message like:

   > “YourAppInstaller.pkg was blocked from use because it is not from an identified developer.”

5. Click **“Open Anyway”**

6. Confirm by clicking **“Open”**

7. The installer will now run normally

---

## Method 3 (Advanced users only)

### Remove Gatekeeper quarantine via Terminal

⚠️ Recommend this **only for technical users**.

### Steps

1. Open **Terminal**

2. Run the command below
   (adjust the path if needed):

```bash
sudo xattr -rd com.apple.quarantine ~/Downloads/YourAppInstaller.pkg
```

3. Enter your macOS password (input will not be visible)

4. Double-click the `.pkg` installer again

---

## Important Notes

* This behavior is part of **macOS Gatekeeper**
* Apple requires a paid Developer Program membership for notarization
* The app itself is unchanged and safe to install
* You do **not** need to disable system security or Gatekeeper

---

## One-line explanation you can show users

> If macOS says the installer is from an unidentified developer, right-click the `.pkg` file and choose **Open**, then confirm. This is a normal macOS security check.
