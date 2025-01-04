### **Module 11: Practical Sessions and Hands-On Projects**

Module 11 focuses on practical skills and real-world applications of accessibility testing. It provides learners with hands-on opportunities to simulate disabilities, test websites and mobile applications for accessibility issues, and conduct real-world accessibility audits.

---

### **1. Simulating Disabilities: Using Tools to Understand User Needs**

#### **Why Simulate Disabilities?**
Simulating disabilities helps testers understand the challenges faced by users with various impairments. It allows them to experience firsthand how accessibility barriers affect users and provides a deeper insight into the impact of accessibility features.

#### **Tools to Simulate Disabilities**:

1. **Screen Reader Simulation**:
   - Use screen readers to simulate the experience of a visually impaired user. Popular screen readers include:
     - **JAWS (Job Access With Speech)**: A widely used screen reader for Windows.
     - **NVDA (Non-Visual Desktop Access)**: A free, open-source screen reader.
     - **VoiceOver**: Built into macOS and iOS, this screen reader helps simulate accessibility for Apple device users.
     - **Narrator**: Windows' built-in screen reader.

2. **Color Blindness Simulators**:
   - Simulate different types of color blindness to understand how users perceive color on a website.
     - **Color Oracle**: A free desktop tool that simulates color blindness.
     - **Coblis**: An online tool that simulates various types of color blindness.
     - **Sim Daltonism**: A macOS app for simulating color blindness.
   - These tools help check if there are any color contrast issues or if users with color blindness face difficulties in distinguishing certain elements.

3. **Keyboard-Only Navigation**:
   - Use the **Tab** key and **Shift + Tab** to navigate through a website or application without a mouse. This simulates the experience of users who rely on keyboard navigation due to motor impairments.
   - Test if all interactive elements are accessible using the keyboard and whether proper focus management is in place.

4. **Text-to-Speech and Speech Recognition**:
   - Use text-to-speech tools like **Natural Reader** or **Speechify** to simulate how people with reading disabilities might engage with web content.
   - Use **Speech-to-Text** tools to test the ease of interacting with web forms or voice-activated features.

5. **Assistive Technology (AT) Simulation**:
   - Tools like **Windows Magnifier** or **ZoomText** simulate low-vision use cases. By using these, you can test how users with partial sight would interact with websites or applications.
   - Use **Dragon NaturallySpeaking** or **Google Assistant** to simulate speech recognition and voice control.

By using these tools, testers can identify where users with disabilities may face difficulties and ensure those issues are resolved to provide an inclusive experience.

---

### **2. Hands-On Testing for Websites and Mobile Applications**

#### **Website Testing**:

1. **Manual Testing**:
   - Navigate the website using keyboard-only controls to identify accessibility issues with focus, links, and form fields.
   - Ensure all content is accessible to screen readers, and check for proper HTML semantics (headings, lists, forms).
   - Validate color contrast ratios using the **Color Contrast Analyzer**.

2. **Automated Testing**:
   - Use tools like **aXe**, **Lighthouse**, and **WAVE** to run automated accessibility tests.
   - Generate reports from these tools to identify potential issues such as missing alt text, improper use of ARIA roles, and accessibility violations.

3. **User Testing**:
   - Conduct real-world user testing with individuals who have disabilities. This can involve screen reader users, users with mobility impairments, and others.
   - Observe how users interact with the website, identify pain points, and collect feedback for improvement.

#### **Mobile Application Testing**:

1. **Native Mobile App Accessibility**:
   - Test mobile apps for accessibility using the built-in tools provided by Android and iOS:
     - **Android**: Use **TalkBack** for screen reader testing and **Accessibility Scanner** for identifying accessibility issues.
     - **iOS**: Use **VoiceOver** for screen reader testing and the **Accessibility Inspector**.

2. **Mobile Web Accessibility**:
   - Test mobile websites to ensure that they are responsive and have accessible touch targets, font sizes, and navigation elements.
   - Simulate various disabilities using mobile simulators and accessibility features in both Android and iOS.

---

### **3. Identifying and Fixing Accessibility Issues**

#### **Identifying Accessibility Issues**:

1. **Manual Inspection**:
   - Check for common accessibility issues such as:
     - Missing or incorrect alt text for images.
     - Improper heading structure or lack of semantic HTML.
     - Form fields without labels or error messages.
     - Poor color contrast or non-descriptive color use.
     - Videos without captions or audio descriptions.

2. **Using Accessibility Testing Tools**:
   - Use automated tools like **aXe**, **WAVE**, **Lighthouse**, or **Tenon** to run scans of the website or mobile application.
   - Analyze the reports to identify specific violations of accessibility standards (WCAG 2.x).

3. **User Feedback**:
   - Collect feedback from users with disabilities to identify issues that may not be easily detected through automated testing. This could include navigation difficulties, content readability, or issues with assistive technology.

#### **Fixing Accessibility Issues**:

1. **Improving Visual Accessibility**:
   - Ensure text has a high contrast ratio against the background. Use online tools like **Color Contrast Analyzer** to check contrast levels.
   - Implement accessible design practices such as:
     - Avoiding color-only indicators (e.g., "red means stop").
     - Providing clear instructions and error messages for forms.
   
2. **Optimizing Keyboard Accessibility**:
   - Ensure all interactive elements (links, buttons, form fields) are focusable using the keyboard.
   - Add appropriate `aria-live` regions to ensure dynamic content updates are announced by screen readers.
   - Manage focus properly, ensuring it moves logically through the page and is returned to the correct position after actions like submitting forms or opening dialogs.

3. **Improving Media Accessibility**:
   - Provide text alternatives like captions for videos and transcripts for audio content.
   - Use ARIA roles such as `role="dialog"` or `role="alert"` for dynamic content like modal windows or error messages.

4. **Ensuring Mobile Accessibility**:
   - Ensure all touch targets are large enough to be easily tapped, with sufficient spacing.
   - Ensure that all interactive elements are accessible via VoiceOver and TalkBack for users with visual impairments.
   
---

### **4. Real-world Project: Conducting Accessibility Audit for a Website**

#### **Steps to Conduct an Accessibility Audit**:

1. **Choose a Website**:
   - Select a website (preferably one that you are familiar with) to audit. This could be a real client website, a personal project, or a public website.

2. **Pre-Audit Preparation**:
   - Understand the scope of the audit. Decide whether you are conducting a full audit or focusing on specific areas like WCAG compliance or screen reader testing.

3. **Initial Assessment**:
   - Conduct an initial assessment using both manual inspection and automated tools (e.g., **aXe**, **WAVE**, **Lighthouse**).
   - Document the areas where the website does not meet accessibility standards.

4. **Analysis and Reporting**:
   - Create a detailed report documenting the accessibility issues found, including severity levels (critical, high, medium, low).
   - Suggest fixes for each issue, prioritizing the most critical ones first.

5. **Implement Fixes**:
   - Implement the recommended fixes, whether through HTML updates, CSS adjustments, or JavaScript changes.
   - For example, adding alt text for images, improving form labels, fixing color contrast, or ensuring keyboard navigation.

6. **Follow-up Testing**:
   - After implementing fixes, re-test the website to ensure that the issues have been resolved.
   - Verify that the website now complies with WCAG 2.x standards or the chosen accessibility guidelines.

7. **User Testing**:
   - Conduct user testing with real users, particularly those with disabilities, to validate the changes and ensure the site is accessible.

8. **Final Report**:
   - Provide a final report summarizing the changes made and ensuring that the website now meets accessibility standards.

---

### **Conclusion**

Module 11 equips learners with practical skills necessary for accessibility testing. By simulating disabilities, testing websites and mobile applications, identifying issues, and conducting real-world audits, learners will gain valuable experience in making digital products accessible for all users. The hands-on approach ensures that learners are not only familiar with theoretical concepts but also capable of implementing accessibility best practices in real-world scenarios.
