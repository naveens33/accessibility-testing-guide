**Module 7: Document Accessibility Testing**

This module focuses on how to test the accessibility of documents such as PDFs, Word, Excel, and PowerPoint, which are commonly used in professional environments. Ensuring that these documents are accessible helps people with disabilities, particularly those who use screen readers or other assistive technologies, to access information.

### **1. Testing PDFs for Accessibility**

**PDF Accessibility** is crucial for documents shared digitally, especially for people using screen readers or braille devices. Accessible PDFs must have logical reading order, alternative text for images, proper heading structure, accessible tables, and form fields that can be navigated by keyboard.

#### **Tools for PDF Accessibility Testing**

1. **Adobe Acrobat Accessibility Checker**
   - Adobe Acrobat provides an **Accessibility Checker** to evaluate and improve the accessibility of PDFs.
   - **Steps**:
     - Open the PDF in **Adobe Acrobat Pro DC**.
     - Go to **Tools** > **Accessibility**.
     - Click on **Full Check** to run the accessibility check.
     - Review the results and use the suggestions to improve accessibility, such as adding alternative text to images, correcting reading order, and adding document tags.
   
2. **PAC 3 (PDF Accessibility Checker)**
   - **PAC 3** is an open-source tool for checking PDF accessibility.
   - **Steps**:
     - Download **PAC 3** from [here](https://www.accessibility.de/en/pdf/).
     - Open the PDF file in PAC 3 and analyze the results.
     - It provides detailed reports on common PDF accessibility issues, like missing alternative text or improper tagging.

3. **Common PDF Accessibility Issues**:
   - **Missing Alternative Text** for images or other non-text content.
   - **Incorrect Reading Order**: Ensure content is read in a logical order.
   - **Lack of Table Structure**: Tables must be properly tagged with row and column headers.
   - **Forms**: Ensure form fields are properly labeled and accessible by keyboard.

---

### **2. Testing Word Documents for Accessibility**

**Microsoft Word** documents must adhere to accessibility guidelines to ensure they are usable by all, especially individuals with visual or cognitive impairments. This includes proper heading structure, alternative text for images, and table accessibility.

#### **Tools for Word Accessibility Testing**

1. **Microsoft Word Accessibility Checker**
   - **Steps**:
     - Open the Word document.
     - Go to the **Review** tab.
     - Click on **Check Accessibility** to run the accessibility checker.
     - Review the results, which include issues like missing alternative text, improper heading structure, and inaccessible tables.
   
2. **Common Word Accessibility Issues**:
   - **Missing Alt Text** for images.
   - **Improper Heading Structure**: Use proper headings (e.g., Heading 1, Heading 2) for document structure.
   - **Tables**: Ensure that tables are tagged correctly with headers for rows and columns.
   - **Lists**: Ensure that bulleted or numbered lists are used correctly for screen readers.

---

### **3. Testing Excel Documents for Accessibility**

Excel documents, especially those used for data analysis, need to be accessible for users with visual impairments. This involves ensuring proper use of headings, alternative text for charts, and making sure that the spreadsheet structure is clear and usable via keyboard.

#### **Tools for Excel Accessibility Testing**

1. **Microsoft Excel Accessibility Checker**
   - **Steps**:
     - Open the Excel file.
     - Go to the **Review** tab and click on **Check Accessibility**.
     - The checker will highlight issues like missing alternative text for images, improper use of headings in tables, and unclear worksheet structures.
   
2. **Common Excel Accessibility Issues**:
   - **Missing Alt Text** for charts, graphs, and images.
   - **Improper Table Structure**: Ensure tables are tagged and include headers for rows and columns.
   - **Use of Colors**: Avoid color as the only means of conveying information (e.g., red/green for data).

---

### **4. Testing PowerPoint Documents for Accessibility**

PowerPoint presentations must be accessible to users with disabilities, especially for individuals with visual or auditory impairments. Accessibility in PowerPoint ensures that slides are readable by screen readers, and multimedia content is accessible.

#### **Tools for PowerPoint Accessibility Testing**

1. **Microsoft PowerPoint Accessibility Checker**
   - **Steps**:
     - Open the PowerPoint presentation.
     - Go to the **Review** tab and click on **Check Accessibility**.
     - The checker will highlight common issues such as missing alt text, poor slide structure, and media issues.
   
2. **Common PowerPoint Accessibility Issues**:
   - **Missing Alt Text** for images, charts, and other non-text content.
   - **Inconsistent Slide Layouts**: Ensure that slides follow a consistent layout to make them easier to navigate.
   - **Audio/Video Content**: Ensure that multimedia content includes captions or transcripts where applicable.
   - **Reading Order**: Ensure the slide content has a logical reading order that works for screen readers.

---

### **5. Ensuring Accessible Forms and Tables in Documents**

#### **Forms Accessibility**:
1. **Microsoft Word and PDF Forms**: 
   - Forms must be fully navigable by keyboard (no mouse reliance).
   - Form fields should be labeled correctly for screen readers.
   - Labels should be associated with form elements, such as text fields, radio buttons, and checkboxes.

2. **Accessible PDF Forms**:
   - Use **Acrobat Pro DC** to ensure form fields are tagged and that labels are linked to the fields.
   - Use the **Tagging tool** to properly tag the form fields and the reading order.
   
3. **Common Issues in Forms**:
   - Missing or misaligned labels for form fields.
   - Fields that cannot be accessed by keyboard (ensure form navigation works via the **Tab** key).
   - Missing instructions for form completion.

#### **Tables Accessibility**:
1. **Microsoft Word, Excel, and PDF Tables**:
   - Tables should have clearly defined headers for rows and columns.
   - Use the **Table Properties** feature to tag headers.
   - In PDFs, ensure tables are properly tagged with header rows and columns.
   
2. **Accessible Tables**:
   - Use clear, concise table data with proper row and column headers.
   - Tables should be structured so that screen readers can read them properly, with a logical flow of data.

3. **Common Issues with Tables**:
   - Missing headers or misaligned rows and columns.
   - Tables that are too complex without proper structure for screen readers to interpret.

---

### **6. Additional Resources for Document Accessibility Testing**

- [WebAIM: PDF Accessibility](https://webaim.org/standards/pdfs/)
- [Microsoft Accessibility Docs](https://www.microsoft.com/en-us/accessibility/)
- [Deque Systems: PDF Accessibility](https://www.deque.com/axe/pdf/)
- [PDF Accessibility Checker (PAC 3)](https://www.accessibility.de/en/pdf/)

### **Conclusion**
Document accessibility is a critical component of making content usable for everyone, including those with disabilities. Testing for accessibility in documents like PDFs, Word, Excel, and PowerPoint can be automated and improved using tools like **Adobe Acrobat Accessibility Checker**, **Microsoft Accessibility Checker**, and open-source tools like **PAC 3**.
