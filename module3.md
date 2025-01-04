### **Module 3: Accessibility Testing Techniques and Tools**

This module introduces the techniques and tools for performing accessibility testing, covering manual and automated approaches, along with real-world examples and practical demonstrations.

---

#### **1. Accessibility Testing Techniques**

##### **a. Manual Testing**
Manual testing involves human interaction to evaluate the accessibility of a digital platform. It identifies usability and contextual issues that automated tools may overlook.

**Steps:**
1. **Keyboard Navigation Testing**:
   - Test navigation using only the keyboard (Tab, Enter, and Arrow keys).
   - **Real-world Scenario**:
     - On a form, check if pressing the "Tab" key moves focus sequentially through input fields and buttons.
   
2. **Screen Reader Testing**:
   - Use screen readers like JAWS or NVDA to test how content is announced.
   - **Example**:
     - A visually impaired user relies on VoiceOver. If a website's buttons are labeled only as "Click here," the screen reader fails to convey meaningful context.

3. **Color Contrast Testing**:
   - Verify if text and background have sufficient contrast to ensure readability.
   - **Example**:
     - Check if a light gray text on a white background meets WCAG’s minimum contrast ratio of 4.5:1.

4. **Testing with Assistive Technologies**:
   - Use magnifiers, voice recognition, and alternative input devices.
   - **Example**:
     - Test a sip-and-puff system for navigating menus.

5. **Empathy Testing**:
   - Simulate challenges faced by users with disabilities, like using a website without a mouse or in grayscale mode.
   - **Example**:
     - Enable high-contrast mode and evaluate usability.

##### **b. Automated Testing**
Automated tools help identify common accessibility issues quickly but should complement manual testing for comprehensive coverage.

**Steps:**
1. **Run Accessibility Scans**:
   - Use tools like Axe or Wave to analyze web pages.
2. **Check Semantic Structure**:
   - Ensure correct HTML structure (headings, landmarks).
3. **Analyze Reports**:
   - Prioritize and address high-severity issues flagged by tools.

---

#### **2. Accessibility Testing Tools**

##### **a. Automated Tools**
1. **Axe by Deque Systems**:
   - Browser extension to identify WCAG violations.
   - **Example**:
     - Detects missing alt attributes on images.

2. **Wave by WebAIM**:
   - Highlights accessibility errors visually on web pages.
   - **Example**:
     - Identifies missing form labels.

3. **Lighthouse (Google)**:
   - Integrated into Chrome DevTools for accessibility audits.
   - **Example**:
     - Provides scores for accessibility, including contrast issues.

4. **Tenon.io**:
   - API-based testing tool for integrating accessibility into CI/CD pipelines.

##### **b. Manual Testing Tools**
1. **Screen Readers**:
   - NVDA, JAWS, VoiceOver.
2. **Color Contrast Checkers**:
   - Contrast Ratio Checker by WebAIM.
   - **Example**:
     - Ensures text on a button meets contrast guidelines.
3. **Keyboard Testing**:
   - Use browser tools to visualize focus outlines.

##### **c. Specialized Tools**
1. **ARIA Validator**:
   - Verifies ARIA roles and attributes for accuracy.
2. **CSS Tools**:
   - Tools like tota11y highlight issues with visual elements.

---

#### **3. Common Accessibility Issues and Fixes**

1. **Missing Alt Text**:
   - **Issue**: Images without alt attributes are inaccessible to screen readers.
   - **Fix**: Add descriptive alt text.
   - **Real-world Example**:
     - On an e-commerce site, "alt='Red sneakers, size 10'" describes a product image.

2. **Inaccessible Forms**:
   - **Issue**: Missing labels for form inputs.
   - **Fix**: Use `<label>` tags and associate them with inputs using the `for` attribute.

3. **Poor Color Contrast**:
   - **Issue**: Low contrast between text and background.
   - **Fix**: Adjust colors to meet WCAG contrast ratios.

4. **Keyboard Navigation Issues**:
   - **Issue**: Focus order is illogical.
   - **Fix**: Ensure elements follow a logical tab order using `tabindex`.

5. **Improper ARIA Roles**:
   - **Issue**: Misused ARIA roles confuse assistive technologies.
   - **Fix**: Use ARIA roles only when needed and correctly.

---

#### **4. Practical Testing Workflows**

**Scenario**: Testing an E-commerce Website
1. **Prepare**:
   - Use a browser extension like Axe.
   - Simulate users with disabilities by enabling assistive technologies.
2. **Test**:
   - Run Axe to identify WCAG violations.
   - Test keyboard navigation for adding items to the cart.
   - Use VoiceOver to verify product descriptions.
3. **Analyze**:
   - Review automated reports and compare them with manual observations.
4. **Fix**:
   - Update code to resolve issues.
5. **Validate**:
   - Re-test after fixes to ensure compliance.

---

#### **5. Role of Accessibility Testing in Agile Development**
- **Inclusion in Sprints**: Integrate accessibility testing in early development stages.
- **Real-world Scenario**:
  - A development team for an educational app conducts accessibility audits during each sprint to ensure compliance before release.

---

#### **Learning Objectives**
By the end of this module, learners will:
1. Differentiate between manual and automated accessibility testing.
2. Use popular accessibility tools to identify and fix issues.
3. Incorporate accessibility testing into development workflows.

---

#### **Activities and Assignments**
1. **Tool Demonstration**:
   - Use Axe or Wave to test a website of choice.
2. **Bug Identification**:
   - Report three accessibility issues and suggest fixes.
3. **Hands-On Testing**:
   - Simulate keyboard-only navigation for a sample web page.

---

### **1. Accessibility Testing Techniques**
#### References:
1. **Web Content Accessibility Guidelines (WCAG) 2.1**  
   - The primary resource for understanding accessibility principles and success criteria.  
   - [WCAG Overview](https://www.w3.org/WAI/standards-guidelines/wcag/)

2. **Keyboard Accessibility Resources**  
   - Guide to ensuring keyboard usability on web interfaces.  
   - [Keyboard Accessibility by WAI](https://www.w3.org/WAI/test-evaluate/preliminary/#keyboard)

3. **Color Contrast Guidelines**  
   - Contrast ratio evaluation tools and tips for compliance.  
   - [Contrast Checker by WebAIM](https://webaim.org/resources/contrastchecker/)

---

### **2. Accessibility Testing Tools**
#### Free Tools:
1. **Axe Browser Extension**  
   - Identify accessibility issues directly within your browser.  
   - [Axe by Deque Systems](https://www.deque.com/axe/)

2. **WAVE Web Accessibility Evaluation Tool**  
   - Visual representation of accessibility issues on websites.  
   - [WAVE Tool](https://wave.webaim.org/)

3. **Lighthouse (Google)**  
   - Built into Chrome DevTools for automated audits.  
   - [Using Lighthouse for Accessibility](https://developer.chrome.com/docs/lighthouse/accessibility/)

4. **NVDA Screen Reader (Windows)**  
   - Free and widely used screen reader.  
   - [Download NVDA](https://www.nvaccess.org/)

#### Paid Tools:
1. **JAWS Screen Reader**  
   - Industry-standard screen reader for accessibility testing.  
   - [JAWS by Freedom Scientific](https://www.freedomscientific.com/products/software/jaws/)

2. **Tenon.io**  
   - API-based accessibility testing solution for CI/CD pipelines.  
   - [Tenon.io Official Site](https://tenon.io/)

3. **SortSite by Powermapper**  
   - Comprehensive accessibility, usability, and SEO testing tool.  
   - [SortSite Accessibility Tool](https://www.powermapper.com/products/sortsite/)

---

### **3. Real-World Case Studies and Examples**
#### a. Practical Guides:
- **Inclusive Design Principles**  
  - Principles and examples to guide accessible design decisions.  
  - [Inclusive Design Principles](https://inclusivedesignprinciples.org/)

#### b. Case Studies:
1. **BBC Accessibility Practices**  
   - Insights into how BBC builds accessible products and services.  
   - [BBC Accessibility](https://www.bbc.co.uk/accessibility/)

2. **GOV.UK Accessibility Team Blog**  
   - Detailed documentation on government website accessibility practices.  
   - [GOV.UK Accessibility Blog](https://accessibility.blog.gov.uk/)

3. **Deque Case Studies**  
   - Real-world applications of accessibility testing and fixes.  
   - [Deque Case Studies](https://www.deque.com/resources/case-studies/)

---

### **4. Training Resources**
#### Tutorials and Courses:
1. **Deque University**  
   - Comprehensive training in accessibility and tools.  
   - [Deque University](https://dequeuniversity.com/)

2. **W3C Accessibility Curriculum**  
   - Free tutorials covering various accessibility topics.  
   - [W3C Accessibility Curriculum](https://www.w3.org/WAI/curricula/)

3. **WebAIM Training**  
   - In-depth training sessions on web accessibility.  
   - [WebAIM Training](https://webaim.org/training/)

#### Books:
1. **"Designing for Accessibility" by Sarah Horton and Whitney Quesenbery**  
   - Practical strategies for implementing accessibility in design.

2. **"Accessibility for Everyone" by Laura Kalbag**  
   - A beginner-friendly guide to web accessibility.

---

### **5. Useful Plugins and Developer Tools**
1. **Accessibility Insights for Web**  
   - Free tool for fast and automated accessibility testing.  
   - [Accessibility Insights](https://accessibilityinsights.io/)

2. **tota11y**  
   - A toolkit for visualizing accessibility issues on a page.  
   - [Download tota11y](https://khan.github.io/tota11y/)

3. **HeadingsMap Chrome Extension**  
   - Analyze heading structures for better navigation.  
   - [HeadingsMap Extension](https://chrome.google.com/webstore/detail/headingsmap/)

---

### **6. Community and Support**
1. **WebAIM Discussion List**  
   - Engage with experts and ask questions about accessibility.  
   - [Join the WebAIM Discussion](https://webaim.org/discussion/)

2. **A11y Project**  
   - A community-driven effort to make accessibility easier to implement.  
   - [The A11y Project](https://www.a11yproject.com/)

---

### **Popular Tools for Manual and Automated Accessibility Testing**

---

### **1. Manual Testing Tool: NVDA (NonVisual Desktop Access)**

#### **Overview**:
NVDA is a free and open-source screen reader for Windows. It reads text on the screen aloud and allows testers to understand how a visually impaired user interacts with applications or websites.

---

#### **Steps for Testing with NVDA**:

1. **Download and Install**:
   - Download NVDA from the official site: [NVDA Download](https://www.nvaccess.org/).
   - Install the software on your Windows system.

2. **Learn Basic Commands**:
   - Familiarize yourself with essential NVDA commands:
     - `Insert + Down Arrow`: Start reading continuously.
     - `Insert + Tab`: Read the currently focused item.
     - `Tab`: Navigate through interactive elements.

3. **Activate NVDA**:
   - Launch NVDA and let it start narrating the screen elements.

4. **Testing Workflow**:
   - **Verify Focus Management**:
     - Tab through elements like forms, buttons, and links.
     - NVDA should announce the name and purpose of each element.
   - **Check Image Descriptions**:
     - Navigate to images and listen for the alt text.
     - **Example Issue**: NVDA announces “Image” without context if alt text is missing.
   - **Test Dynamic Content**:
     - Interact with modals, dropdowns, and pop-ups to see if NVDA announces updates correctly.

5. **Analyze Feedback**:
   - Note any elements NVDA cannot interpret or where the navigation sequence breaks.
   - Ensure all meaningful content is accessible.

---

#### **Real-World Example**:
**Scenario**: Testing a government website.  
- Navigate the site using NVDA and verify announcements for menus, forms, and interactive widgets.
- Identify issues like unlabeled form fields or inaccessible dropdowns.

---

### **2. Automated Testing Tool: Axe by Deque Systems**

#### **Overview**:
Axe is a popular automated accessibility testing tool. It is available as a browser extension (Chrome and Firefox) and integrates with development tools for accessibility audits.

---

#### **Steps for Testing with Axe**:

1. **Install Axe**:
   - Download the Axe extension for your browser:
     - [Axe for Chrome](https://chrome.google.com/webstore/detail/axe/lhdoppojpmngadmnindnejefpokejbdd)
     - [Axe for Firefox](https://addons.mozilla.org/en-US/firefox/addon/axe-devtools/)

2. **Open a Web Page**:
   - Navigate to the page you want to test.

3. **Activate Axe**:
   - Open browser Developer Tools (right-click > Inspect or `Ctrl + Shift + I`).
   - Navigate to the Axe tab in the DevTools panel.

4. **Run an Audit**:
   - Click the “Analyze” button in the Axe panel.
   - Axe scans the page and displays a list of accessibility issues.

5. **Review Results**:
   - **Categories of Issues**:
     - Critical: High-severity issues like missing alt text or improper ARIA roles.
     - Serious: Navigation problems or color contrast violations.
   - Each issue includes:
     - A description of the problem.
     - Location in the DOM.
     - Recommended fix.

6. **Fix and Validate**:
   - Resolve issues in the code (e.g., add missing alt attributes, fix ARIA roles).
   - Rerun Axe to verify fixes.

---

#### **Real-World Example**:
**Scenario**: Testing an e-commerce website.  
- Run Axe to detect accessibility violations.
- Example Issue: Missing form labels for checkout fields.
- Resolution: Add descriptive labels using the `<label>` tag.

---

#### **Key Features of Axe**:
- Integrates with CI/CD pipelines for automated testing.
- Provides clear guidance for developers to fix issues.
- Compatible with WCAG 2.1 standards.

---

### **Comparison of NVDA and Axe**

| Feature                  | NVDA (Manual)                                      | Axe (Automated)                                    |
|--------------------------|---------------------------------------------------|---------------------------------------------------|
| **Purpose**              | Test user experience with screen readers.         | Detect code-level accessibility issues.           |
| **Strengths**            | Simulates real user behavior; tests dynamic content. | Fast issue detection; integrates with workflows. |
| **Weaknesses**           | Time-consuming; requires manual effort.           | Misses contextual or usability problems.          |
| **Ideal Use Case**       | Verifying user-facing issues (e.g., screen reader compatibility). | Initial audits and regression testing.            |

---

### **Reference Links**:
- **NVDA Official Site**: [NVDA](https://www.nvaccess.org/)
- **Axe by Deque Systems**: [Axe](https://www.deque.com/axe/)  
- **WCAG Guidelines**: [WCAG Overview](https://www.w3.org/WAI/standards-guidelines/wcag/)  
- **Deque Axe Tutorials**: [Axe Tutorials](https://www.deque.com/axe/tools/)

---
