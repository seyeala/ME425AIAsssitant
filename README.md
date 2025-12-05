# ME425 Course Assistant – Terms of Use & Privacy Policy

_Last updated: {{insert date}}_

The **ME425 Course Assistant** (“the Assistant”) is an educational tool to support students enrolled in **ME 425: Applied Deep Learning for Mechanical Engineering** at **New Mexico State University**. It helps students review course materials, understand key concepts, and optionally send anonymous course-related feedback to the instructor.

By using the Assistant, you agree to the Terms of Use and Privacy Policy described in this document, in addition to the terms of any third-party platforms involved (such as OpenAI and Google).

---

## 1. Purpose of the Assistant

The Assistant is designed to:

- Help students understand lecture slides, notes, and other ME 425 materials.
- Provide explanations, summaries, and short practice quizzes.
- Offer limited conceptual guidance related to course topics.
- Optionally send **anonymous course feedback** to the instructor via a dedicated feedback endpoint.

The Assistant is **not** a grading tool, exam solver, or replacement for attending lectures, reading materials, or communicating directly with the instructor.

---

## 2. Acceptable Use

You may use the Assistant to:

- Clarify ME 425 course concepts and terminology.
- Review lecture content and notes.
- Request summaries of specific sections, topics, or lectures.
- Generate small self-test quizzes (e.g., 3–6 questions) for practice.
- Ask for help understanding mathematical expressions or deep learning concepts covered in ME 425.
- Submit anonymous, course-related concerns or feedback via the feedback feature.

You agree to use the Assistant **respectfully** and in accordance with NMSU policies and applicable laws.

---

## 3. Prohibited Use & Academic Integrity

You may **not** use the Assistant to:

- Obtain full solutions or direct answers to **graded** homework, quizzes, exams, or projects.
- Circumvent academic integrity rules or assist others in doing so.
- Ask for specific answers to take-home or online assessments that count toward your grade.
- Provide sensitive personal information (about yourself or others) that is not necessary for learning.
- Misuse or spam the anonymous feedback channel.

The Assistant is configured to refuse requests that appear to violate academic integrity, but **you remain responsible** for your own conduct under university policies.

Use of the Assistant does **not** override any ME 425 syllabus rules, departmental policies, or NMSU academic integrity regulations.

---

## 4. No Guarantee of Accuracy or Completeness

The Assistant:

- May generate **incorrect or incomplete** information.
- May misinterpret or oversimplify concepts.
- May not fully reflect the instructor’s intent or emphasis.
- Cannot see updates made to course materials unless those are provided to it.

You must:

- Treat all explanations as **informational**, not authoritative.
- Verify important details with official course materials (slides, notes, assignments) and/or the instructor.
- Understand that use of the Assistant **does not guarantee** improved grades or mastery of the subject.

The instructor and university are **not responsible** for decisions you make based on Assistant responses.

---

## 5. Anonymous Feedback Feature

### 5.1 Purpose

The Assistant includes an **optional** anonymous feedback feature to allow students to share course-related concerns or suggestions with the instructor (Dr. Amin Alaie) in a way that does not reveal their identity.

This feature is intended for:

- Feedback about course pace, clarity of materials, or assessments.
- Classroom environment or learning experience feedback.
- Suggestions for improvements.

It is **not** a replacement for official reporting channels for serious issues.

---

### 5.2 How Anonymous Feedback Works

When you choose to send anonymous feedback:

1. The Assistant asks for your permission (e.g., “Would you like me to send this as an anonymous concern to Dr. Alaie?”).
2. The Assistant **summarizes** your concern and attempts to remove direct identifiers (such as names, emails, IDs), unless you explicitly state that you want to be contactable.
3. The Assistant sends this summary via a secure HTTP POST to a Google Apps Script endpoint:
   - `https://script.google.com/macros/s/AKfycbwknb6PMnHJch1iLG86d5sAmlorJf9jFLapbpSpN1HT8C2B6Vl6KX1A4Ui0eOyw9Mk/exec`
4. The script generates an email to the instructor with:
   - The anonymized message.
   - A category (e.g., course pace, clarity of materials, assessment fairness, course environment, other).
   - A flag indicating whether you requested a reply (`student_wants_reply: true/false`).

The instructor sees **only** the anonymized content and category; they do **not** see your name or account details from the Assistant.

---

### 5.3 What Is and Isn’t Sent in Feedback

**Sent to the instructor (via email):**

- An anonymized summary of your concern (“message”).
- A category describing the type of concern.
- Whether you requested a reply (`student_wants_reply`).

**Not intentionally sent:**

- Your name.
- Your email address or NMSU login.
- Your student ID.
- Your full chat history.
- Technical metadata that identifies you (such as device information).

If you type identifying details directly into your message (e.g., “This is John Doe, please email me at ___”), those may appear in the anonymized summary. You are responsible for deciding whether to include that information.

The Assistant will inform you that **“Dr. Alaie will not know who submitted this”** unless you explicitly choose to identify yourself.

---

### 5.4 Limitations of Anonymity

Although the system is **designed** to keep feedback anonymous:

- No digital system can guarantee absolute anonymity.
- Third-party tools (OpenAI, Google, NMSU systems) may maintain internal logs or metadata outside the instructor’s control.
- You should **avoid including unnecessary identifying details** in the feedback text.

For **serious, urgent, safety-related, or harassment/discrimination issues**, you should use official university reporting channels rather than relying solely on anonymous feedback through this tool.

---

## 6. Privacy – Information Collected and Not Collected

### 6.1 Information the Assistant Does Not Automatically Collect

The Assistant itself does **not** automatically collect or store:

- Your name.
- Your email address.
- Your NMSU username or student ID.
- Files or documents from your device.
- Location or device identifiers.

The Assistant operates within the OpenAI platform environment and does not add any separate database or tracking on top of that.

---

### 6.2 Information Processed During Use

During normal use, the following types of data may be processed:

- The text you type into the Assistant (questions, feedback, etc.).
- The Assistant’s generated responses.
- Anonymous feedback summaries, if you choose to send them.

These are processed:

- By OpenAI (to generate responses and operate the GPT platform), under OpenAI’s terms and privacy policy.
- By Google’s infrastructure (for the Apps Script feedback endpoint and email delivery).

The instructor does not operate additional tracking outside these systems, beyond receiving anonymized feedback emails.

---

### 6.3 Data Handling and Storage

- **Assistant chats** are processed and may be retained by OpenAI in accordance with its policies:  
  See: https://openai.com/policies
- **Anonymous feedback emails** are delivered to the instructor’s university email account and may be kept as part of normal email retention practices.
- The instructor does **not** maintain a separate database of identifiable student usage logs from the Assistant.

Students should not use this tool to transmit highly sensitive or legally protected personal information.

---

## 7. Third-Party Services and Platform Terms

By using the Assistant, you acknowledge that it relies on the services of third parties, whose policies apply **in addition** to this document.

### 7.1 OpenAI

All interactions with the Assistant occur through the **OpenAI** platform (or related interfaces).  
By using the Assistant, you agree that:

- Your input and the Assistant’s responses are processed by OpenAI systems.  
- OpenAI’s Terms of Use, Privacy Policy, and Usage Policies apply.  
- OpenAI may log, store, or analyze interactions for safety and product improvement consistent with its policies.

You should review OpenAI’s current policies at:  
https://openai.com/policies

---

### 7.2 Google (Apps Script & Email)

The anonymous feedback feature uses **Google Apps Script** and **Gmail** to send messages to the instructor.

By using this feature, you understand that:

- The feedback endpoint runs on Google’s infrastructure.
- Google’s Terms of Service and Privacy Policy apply to that processing.
- Google may maintain infrastructure-level logs in accordance with its own policies.

The script is configured only to receive anonymized JSON (category, message, student_wants_reply) and send an email to the instructor.

For Google’s policies, see:  
https://policies.google.com

---

### 7.3 Combined Effects

Because both OpenAI and Google are involved:

- OpenAI processes your chat messages and decides when to call the feedback tool.
- Google processes the anonymized feedback and email delivery.
- The Assistant does not control, and cannot modify, how these third parties handle infrastructure-level data.

Neither the instructor nor the Assistant can override OpenAI’s or Google’s platform policies.

---

## 8. Legal Disclaimers and Limitations of Liability

### 8.1 No Professional Advice

The Assistant:

- Does not provide legal, medical, mental health, safety, or emergency advice.
- Is not a substitute for professional services or official university guidance.
- Cannot interpret emergency situations or provide crisis intervention.

For emergencies, call local emergency services or use official NMSU channels.

---

### 8.2 No Warranty of Functionality or Availability

The Assistant is provided **“as is”**, with no guarantees that:

- It will be available at all times.
- It will function without interruption or error.
- It will always call the feedback endpoint successfully.
- It will remain unchanged throughout the semester.

Service interruptions may arise from OpenAI, Google, network issues, or institutional IT changes.

---

### 8.3 Limitation of Liability

To the fullest extent permitted by law:

- The instructor, the Mechanical & Aerospace Engineering Department, New Mexico State University, and OpenAI are **not liable** for:
  - Errors or omissions in responses.
  - Misuse of the Assistant by students.
  - Data loss, delays, or email delivery failures.
  - Third-party platform failures or policy changes.
  - Academic, personal, or professional consequences arising from reliance on Assistant output.

Your use of the Assistant is voluntary and at your own risk.

---

### 8.4 Compliance With Laws and University Policies

You agree to use the Assistant in compliance with:

- Federal and state laws.
- NMSU policies and student codes of conduct.
- Departmental and course-level academic integrity rules.
- FERPA and related privacy protections.

The Assistant must **not** be used to transmit or store sensitive personal data (e.g., protected educational records) beyond what is appropriate in normal course communication.

---

### 8.5 No Contractual Relationship

Use of the Assistant:

- Does not create a contract or legal obligation between you and the instructor, department, university, or OpenAI beyond existing institutional and platform terms.
- Does not modify the syllabus, grading policies, or official course requirements.

Official course communications and policies are those issued directly by the instructor or university.

---

## 9. Student Responsibilities and Choices

You, as the user:

- Are responsible for verifying important information with official course materials.
- Are responsible for following all academic integrity rules.
- Should avoid including unnecessary personal identifiers in messages or feedback.
- May choose to:
  - Use the Assistant only for learning (no feedback).
  - Use or decline the anonymous feedback feature.
  - Ask the Assistant **not** to forward a concern.

Anonymous feedback is **optional** and is meant to supplement, not replace, direct communication or official reporting channels.

---

## 10. Modification or Termination of the Assistant

The instructor reserves the right to:

- Modify the Assistant’s capabilities.
- Change or disable the anonymous feedback feature.
- Restrict access at any time.
- Update this Terms of Use & Privacy Policy document.

Changes may occur without prior notice, though reasonable efforts may be made to inform students via course announcements.

---

## 11. Contact

For questions or concerns about this Assistant, its usage, or these policies, contact:

**Dr. Amin Alaie**  
Mechanical & Aerospace Engineering Department  
New Mexico State University  

(Use your official NMSU communication channels.)

---

_End of ME425 Course Assistant – Terms of Use & Privacy Policy_
