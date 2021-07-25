## *Appearance & Behavior*

### **Appearance**

* UI Options

  KEY | VALUE
  --- | -----
  Use smaller indents in trees | ✓
  Enable mnemonics in controls | ✓
  Smooth scrolling | ✓
  Display icons in menu items | ✓

* Tool Windows

  KEY | VALUE
  --- | -----
  Show tool windows bars | ✓
  Show tool windows numbers | ✓

## *Editor*

### **General**

* On Save

  KEY | VALUE
  --- | -----
  Remove trailing spaces on | All lines
  Keep trailing spaces on caret line | ✗
  Remove trailing blank lines at the end of saved lines | ✗
  Ensure every saved file ends with a line break | ✓

### **Auto Import**

* Java

  KEY | VALUE
  --- | -----
  Optimize imports on the fly | ✓

### **Appearance**

  KEY | VALUE
  --- | -----
  Show line numbers | ✓
  Show indent guides | ✓
  Show intention bulb | ✓
  Show code lens on scrollbar hover | ✓
  Render documentation comments | ✓
  Enable HTML/XML tag tree highlighting | ✓

### **Breadcrumbs**

  KEY | VALUE
  --- | -----
  Show breadcrumbs | ✗

### **Code Folding**

  KEY | VALUE
  --- | -----
  Show code folding outline | ✓

* Fold by default

  KEY | VALUE
  --- | -----
  File header | ✓
  Imports | ✓
  Documentation comments | ✓

* Java

  KEY | VALUE
  --- | -----
  One-line methods | ✓
  Closures | ✓
  Generic constructor and method parameters | ✓
  i18n strings | ✓
  @SuppressWarnings | ✓

### **Console**

  KEY | VALUE
  --- | -----
  Use soft wraps in console | ✓

### **Editor Tabs**

* Appearance

  KEY | VALUE
  --- | -----
  Use small font for lables | ✗
  Show file icon | ✓
  Show file extension |  ✗
  Show directory for non-unique file names | ✓
  Mark modified (*) | ✓
  Show full path on mouse hover | ✓

* Tab Order

  KEY | VALUE
  --- | -----
  Open new tabs at the end | ✓

* Opening Policy

  KEY | VALUE
  --- | -----
  Enable preview tab | ✓
  Open declaration source in the same tab | ✓

### **Code Style**

  KEY | VALUE
  --- | -----
  Line separator | Unix and macOS (\n)
  Hard wrap at | 120
  Detect and use existing file indents for editing | ✓
  Enable EditorConfig support | ✓

  * Java

    * Tabs and Indents

      KEY | VALUE
      --- | -----
      Use tab character| ✗
      Tab size | 2
      Indent | 2
      Continuation indent | 2
      Keep indents on empty lines | ✗
      Lable indent | 0
      Absolute label indent | ✗
      Do not indent top level class members | ✗
      Use indent relative to expression start | ✗

    * Imports

      KEY | VALUE
      --- | -----
      Use single class import | ✓
      Layout static imports separately |  ✓

      > Below shows **Import Layout**. 因为以下配置涉及到项目相关的设置，因此我们需要创建一个项目相关的Code Style配置。

      KEY |
      --- |
      import java.*
      import javax.*
      `<blank line>`
      import all other imports
      `<blank line>`
      import static all other imports
      `<blank line>`
      import com.spin.wholesales.*

