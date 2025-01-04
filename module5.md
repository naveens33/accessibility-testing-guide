### **Module 5: Building an Accessible Development and Testing Workflow**

---

### **Overview**  
This module focuses on integrating accessibility practices into the development and testing lifecycle. It includes guidelines for developers, testers, and product managers to collaboratively ensure accessibility is baked into every stage of the software development life cycle (SDLC). We’ll also explore popular tools and frameworks that support accessibility in CI/CD workflows.

---

### **Key Topics in Module 5**

---

#### **1. Embedding Accessibility in the SDLC**  

1. **Planning Stage**:
   - Incorporate accessibility requirements into product specifications.
   - Use **WCAG** as a reference to define the “Definition of Done” for accessibility.

   **Example**:
   - Requirement: All buttons must have descriptive labels (e.g., “Submit Order” instead of “Click Here”).

2. **Design Stage**:
   - Use accessible design principles:
     - High contrast for text and background.
     - Focus indicators for navigation.
     - Sufficient touch target size for mobile interfaces.
   - Tools: 
     - **Adobe XD Accessibility Plugin**: Ensures designs are WCAG-compliant.
     - **Figma Accessibility Plugin**: Provides contrast checking and ARIA guidelines.

3. **Development Stage**:
   - Follow coding standards for accessibility:
     - Use semantic HTML (e.g., `<header>`, `<main>`, `<footer>`).
     - Include ARIA roles where necessary.
     - Ensure forms are accessible with `<label>` and error messages.

   **Real-Time Example**:
   - A login page:
     ```html
     <label for="username">Username</label>
     <input type="text" id="username" aria-required="true">
     ```

4. **Testing Stage**:
   - Conduct both **manual** and **automated** accessibility testing (as discussed in Modules 3 and 4).

5. **Deployment Stage**:
   - Integrate accessibility checks into CI/CD pipelines.

---

#### **2. Accessibility Tools and Frameworks**

1. **Linting Tools for Accessibility**:
   - **eslint-plugin-jsx-a11y**: For React projects.
     - Automatically flags accessibility issues in JSX code.

   **Example**:
   ```javascript
   <img src="image.jpg" /> 
   // Error: Missing alt text for image.
   ```

2. **Browser Extensions**:
   - **Axe DevTools** and **Accessibility Insights**.
     - Use during development to catch issues early.

3. **CI/CD Integration**:
   - **Pa11y CI**: Automates accessibility tests in CI pipelines.
   - **Lighthouse CI**: Google’s tool for checking accessibility scores.

   **Steps for Integration**:
   - Add Pa11y to your pipeline.
   - Configure rules for your project (e.g., WCAG AA compliance).
   - Fail builds if critical accessibility issues are found.

---

#### **3. Automating Accessibility Testing in CI/CD**

1. **Set Up a Workflow**:
   - Include accessibility tools in your build pipeline (e.g., Jenkins, Bitbucket Pipelines, GitHub Actions).

2. **Example Pipeline Configuration**:
   ```yaml
   steps:
     - step: 
         name: Run Accessibility Tests
         script:
           - npm install -g pa11y-ci
           - pa11y-ci
   ```

3. **Monitoring Accessibility Compliance**:
   - Use dashboards to track compliance over time.

---

#### **4. Accessibility for Modern Frameworks**

1. **React**:
   - Use `react-axe` for runtime accessibility checks.
     - [React-Axe Documentation](https://github.com/dequelabs/react-axe)

   **Example**:
   ```javascript
   import axe from 'react-axe';
   if (process.env.NODE_ENV !== 'production') {
     axe(React, ReactDOM, 1000);
   }
   ```

2. **Angular**:
   - Use tools like **Accessibility Developer Tools** to analyze Angular apps.
   - Best Practice: Use `aria-*` attributes for enhanced accessibility.

   **Example**:
   ```html
   <button aria-label="Submit the form">Submit</button>
   ```

---

#### **5. Real-Time Examples of Accessible Workflows**

1. **Case Study: E-Commerce Website**:
   - **Issue**: Missing focus indicators on the checkout form.  
   - **Solution**:
     - Added focus styles in CSS:
       ```css
       button:focus {
         outline: 3px solid #f00;
       }
       ```

   - Implemented Lighthouse CI for automated checks after every deployment.

2. **Case Study: Banking Application**:
   - **Problem**: Inaccessible dropdowns in the loan calculator.  
   - **Fix**:
     - Replaced custom dropdowns with native `<select>` elements.
     - Used Axe to verify compliance.

---

#### **6. Best Practices for Collaboration**  

1. **Developers**:
   - Learn WCAG principles and incorporate accessibility coding standards.

2. **Testers**:
   - Test accessibility early and often.
   - Use screen readers and automated tools together for comprehensive coverage.

3. **Product Managers**:
   - Set clear accessibility goals and include them in project roadmaps.

4. **Designers**:
   - Use accessible color schemes and ensure designs are tested with contrast-checking tools.

---

#### **7. Additional Tools for Accessible Workflows**

| **Tool**                 | **Purpose**                                         | **Link**                                         |
|---------------------------|-----------------------------------------------------|-------------------------------------------------|
| **react-axe**             | Runtime accessibility testing for React apps.       | [react-axe](https://github.com/dequelabs/react-axe) |
| **Pa11y**                 | Automated accessibility testing in CI pipelines.    | [Pa11y](https://pa11y.org/)                    |
| **Deque Axe CLI**         | Accessibility testing in build systems.             | [Axe CLI](https://www.deque.com/axe/)          |
| **Accessibility Insights**| Accessibility testing for Android and web.          | [Accessibility Insights](https://accessibilityinsights.io/) |

---

#### **8. Resources for Learning and Reference**

1. **Official WCAG Guidelines**:  
   - [WCAG Overview](https://www.w3.org/WAI/standards-guidelines/wcag/)  

2. **Deque University** (Training and Resources):  
   - [Deque University](https://dequeuniversity.com/)  

3. **Google Lighthouse Documentation**:  
   - [Lighthouse Accessibility](https://developers.google.com/web/tools/lighthouse/)  

---
