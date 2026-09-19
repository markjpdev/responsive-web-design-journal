# Day 19: Sept 19, 2026 — Build a Survey Form (Certification Project)

### 📝 Today's Progress
Completed and passed the **Build a Survey Form** certification project[cite: 16], assembling a full custom HTML form with inputs, dropdowns, selection controls, and text areas.

### 💡 Key Takeaways

**1. Survey Form Architecture (`<form>`)**  
Constructed a complete survey form featuring text, email, and number inputs alongside custom radio buttons, checkboxes, dropdown `<select>` menus, and a multi-line `<textarea>` comment box[cite: 16].

**2. Form Field Accessibility & Linking**  
Applied unique `id` attributes across inputs (`#name`, `#email`, `#number`, `#dropdown`) and assigned matching explicit `<label>` elements (`#name-label`, `#email-label`, `#number-label`) to ensure proper accessibility compliance[cite: 16].

**3. HTML Code Preservation**  
Saved the raw code structure for future CSS styling reference:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Survey Form</title>
  </head>
  <body>
    <h1 id="title">My First Form</h1>
    <p id="description">This is my first form since first year college</p>
    <form id="survey-form">
      <label id="name-label">Name:</label>
      <input
        id="name"
        type="text"
        placeholder="Enter your Name"
        required
      ><br>

      <label id="email-label">Email:</label>
      <input
        id="email"
        type="email"
        placeholder="Enter your email"
        required
      ><br>

      <label id="number-label">Age (Optional)</label>
      <input
        id="number"
        type="number"
        min="5"
        max="12"
        placeholder="Age"
      ><br><br>

      <p>Are you enjoying the course?</p>
      <select id="dropdown" name="Select current role">
        <option value="Yes">Yes, i am enjoying the course</option>
        <option value="No">No, It's too confusing</option>
      </select><br><br>

      <p>Would you recommend freeCodeCamp to a friend?</p>
      <label>
        <input type="radio" name="choice" value="Definitely" checked>Definitely
      </label>
      <label>
        <input type="radio" name="choice" value="Maybe">Maybe
      </label>
      <label>
        <input type="radio" name="choice" value="No">No
      </label>

      <p>Where do you prefer to study</p>
      <select id="study-place" name="place">
        <option value="Bedroom">Bedroom</option>
        <option value="Livingroom">Living Room</option>
      </select><br><br>

      <p>Which path are you pursuing (Check all that apply)</p>
      <label>
        <input type="checkbox" name="preference" value="Frontend">Frontend
      </label>
      <label>
        <input type="checkbox" name="preference" value="Backend">Backend
      </label>
      <label>
        <input type="checkbox" name="preference" value="Fullstack">Fullstack
      </label>

      <p>Any comments and suggestions?</p>
      <textarea placeholder="Enter your suggestion here"></textarea><br>
      <button type="submit" id="submit">Submit</button>
    </form>
  </body>
</html>
