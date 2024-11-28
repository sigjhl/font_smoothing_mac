# Font Smoothing Setter

Easily adjust or reset font smoothing settings on macOS with a graphical user interface, built using Automator.

---

## **Overview**

**Font Smoothing Setter** is a lightweight macOS app that allows you to adjust your font smoothing preferences or reset them to the default, all via a simple graphical user interface. Built with Automator, this app replicates and restores the functionality removed in macOS Big Sur and later.

---

## **What is Font Smoothing?**

Font smoothing is a feature in macOS that makes text appear slightly bolder by enhancing the edges of characters. While it can improve readability in some cases, it can also blur text and distort the finely tuned shapes of certain fonts.

For more details, see the font smoothing section of [Nikita Prokopov’s article on fonts](https://tonsky.me/blog/monospace/).

---

## **Why Use Font Smoothing Setter?**

In macOS versions prior to Big Sur, you could disable or adjust font smoothing directly from the **System Preferences** > **General** pane. Starting with macOS Big Sur, Apple removed this option, leaving users with only Terminal commands to make adjustments.

This Automator app restores that convenience, providing an easy way to:

- Disable font smoothing entirely.
- Adjust font smoothing to various levels (Light, Medium, Strong).
- Remove all customizations and restore default macOS font smoothing settings.

---

## **Features**

- **Graphical Interface**: No need to use Terminal commands—adjust settings with just a few clicks.
- **Multiple Options**: Choose from four font smoothing levels or reset to the default settings.
- **Lightweight**: Built entirely with Automator and AppleScript, with no third-party dependencies.
- **Safe and Simple**: Executes macOS defaults commands securely.

---

## **How to Download and Use**

1. **Download the App**: *(Provide download link if hosted online.)*
2. **Run the App**:
   - Open the **Font Smoothing Setter** app.
   - Select your desired font smoothing level:
     - **Disable Font Smoothing**
     - **Light Font Smoothing**
     - **Medium Font Smoothing** (Default)
     - **Strong Font Smoothing**
     - **Delete Custom Setting for Font Smoothings**
   - Click **OK** to apply the changes.
3. **Restart Your Mac**: Restart your computer for the changes to take effect.

---

## **Alternative: Terminal Commands**

If you’re comfortable using Terminal, you can manually adjust your font smoothing settings with the following commands:

### **Disable Font Smoothing**:
```bash
defaults -currentHost write -g AppleFontSmoothing -int 0
```

### **Set Light Font Smoothing**:
```bash
defaults -currentHost write -g AppleFontSmoothing -int 1
```

### **Set Medium Font Smoothing (Default)**:
```bash
defaults -currentHost write -g AppleFontSmoothing -int 2
```

### **Set Strong Font Smoothing**:
```bash
defaults -currentHost write -g AppleFontSmoothing -int 3
```

### **Reset to Default Font Smoothing (delete the custom settings completely)**:
```bash
defaults -currentHost delete -g AppleFontSmoothing
```

### **Note**:  
You will need to log off or restart your Mac for the changes to take effect system-wide.

---

## **Credits**

Inspired by the original **Font Smoothing Adjuster** app (https://github.com/bouncetechnologies/Font-Smoothing-Adjuster) and designed to restore the lost font smoothing settings functionality on macOS.

---

## **License**

APACHE 2.0
