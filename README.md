# Syllogiser: A Venn and Euler Diagram Tool for Categorical Logic

Welcome to Syllogiser! This educational platform helps you learn and understand categorical logic through interactive diagrams. Whether you're studying basic propositions or complex syllogistic arguments, this tool provides visual representations to enhance your understanding.

Syllogiser is unique in that it supports both Venn Diagrams and Euler Diagrams, making it a versatile tool for all your logical diagramming needs.

No build process, no dependencies, no server required — it’s a single, self-contained HTML file!

System Requirements
Any modern web browser (Chrome, Firefox, Safari, Edge)
JavaScript enabled
Minimum screen width: 320px (mobile-friendly)
📘 Usage Guide
Statement Mode
Statement Mode is designed for analyzing individual categorical propositions.

Switch to Statement Mode using the toggle at the top of the left panel
Enter terms in the Premise row:
Type the subject term (e.g., “dogs”)
Type the predicate term (e.g., “mammals”)
Select logical operators:
Quantifier: “All” or “Some”
Copula: “are” or “are not”
View the proposition type: The type (A, E, I, O) is automatically displayed
Create a diagram: Use the canvas on the right to visualize the proposition
Copy to Syllogism: Use the copy buttons to transfer premises to Syllogism Mode
Syllogism Mode
Syllogism Mode is designed for analyzing categorical syllogisms.

Switch to Syllogism Mode using the toggle (default mode)
Enter Premise 1:
Subject term (e.g., “men”)
Predicate term (e.g., “mortal”)
Select quantifier and copula
Enter Premise 2:
Subject term (e.g., “Greeks”)
Predicate term (e.g., “men”)
Select quantifier and copula
Select Conclusion terms from the dropdown menus:
The system requires exactly 3 unique terms across both premises
Subject and Predicate dropdowns are populated automatically
Check Validity: Click the Check Validity button to analyze
View Results: See the mood-figure code, traditional name, and validity status
Use System Proving: Click to see detailed rule-by-rule analysis
Creating Diagrams
Basic Operations
Action	Mouse	Touch
Color a region	Click on region	Tap on region
Paint multiple regions	Click and drag	Touch and drag
Move a circle	Drag from center	Touch and drag from center
Resize a circle	Drag from edge	Touch and drag from edge
Move existence marker	Drag the X	Touch and drag the X
Toolbar Functions
Color Palette: Select a color before clicking on regions
Clear All: Remove all coloring from the diagram
Add Existence: Place an X marker on the canvas
Clear Existence: Remove all X markers
Boolean/Aristotelian Toggle: Switch logic systems
Tips for Effective Diagrams
Use Diagram 1 for premise visualization
Use Diagram 2 for conclusion or comparison
For Euler diagrams: resize and reposition circles to show containment or exclusion
For Venn diagrams: shade regions to show empty sets
The transparent color (white button) acts as an eraser
Sorites (Chain Syllogisms)
Syllogiser supports the analysis of sorites through copy functions:

In Statement Mode:
“Premise → Syllogism P1”: Copies current statement to Premise 1
“Premise → Syllogism P2”: Copies current statement to Premise 2
In Syllogism Mode:
“Conclusion → P1”: Copies the conclusion to Premise 1 for chaining
Workflow for Sorites:
Analyze first pair of premises
Check validity
Copy conclusion to P1
Enter next premise in P2
Repeat until final conclusion
📚 Valid Syllogistic Forms
Unconditionally Valid Forms (15 total)
These forms are valid in both Boolean and Aristotelian logic.

Figure 1 (M–P, S–M)
Mood	Name	Major Premise	Minor Premise	Conclusion
AAA	Barbara	All M are P	All S are M	All S are P
EAE	Celarent	No M are P	All S are M	No S are P
AII	Darii	All M are P	Some S are M	Some S are P
EIO	Ferio	No M are P	Some S are M	Some S are not P
Figure 2 (P–M, S–M)
Mood	Name	Major Premise	Minor Premise	Conclusion
EAE	Cesare	No P are M	All S are M	No S are P
AEE	Camestres	All P are M	No S are M	No S are P
EIO	Festino	No P are M	Some S are M	Some S are not P
AOO	Baroco	All P are M	Some S are not M	Some S are not P
Figure 3 (M–P, M–S)
Mood	Name	Major Premise	Minor Premise	Conclusion
IAI	Disamis	Some M are P	All M are S	Some S are P
AII	Datisi	All M are P	Some M are S	Some S are P
OAO	Bocardo	Some M are not P	All M are S	Some S are not P
EIO	Ferison	No M are P	Some M are S	Some S are not P
Figure 4 (P–M, M–S)
Mood	Name	Major Premise	Minor Premise	Conclusion
AEE	Camenes	All P are M	No M are S	No S are P
IAI	Dimaris	Some P are M	All M are S	Some S are P
EIO	Fresison	No P are M	Some M are S	Some S are not P
Conditionally Valid Forms (9 total)
These forms are valid only in Aristotelian logic (assuming existential import).

Figure 1
Mood	Name	Condition
AAI	Barbari	Requires S to exist
EAO	Celaront	Requires S to exist
Figure 2
Mood	Name	Condition
EAO	Cesaro	Requires S to exist
AEO	Camestros	Requires S to exist
Figure 3
Mood	Name	Condition
AAI	Darapti	Requires M to exist
EAO	Felapton	Requires M to exist
Figure 4
Mood	Name	Condition
AAI	Bramantip	Requires P to exist
EAO	Fesapo	Requires M to exist
AEO	Calemos	Requires S to exist
🛠 Technical Details
Technologies Used
HTML5: Semantic markup and structure
CSS3: Modern styling with flexbox, gradients, and transitions
Vanilla JavaScript: No frameworks or libraries required
HTML5 Canvas: Hardware-accelerated diagram rendering
Browser Support
Browser	Version	Status
Chrome	80+	Fully Supported
Firefox	75+	Fully Supported
Safari	13+	Fully Supported
Edge	80+	Fully Supported
iOS Safari	13+	Fully Supported
Chrome Android	80+	Fully Supported
File Structure
text
syllogiser/
├── index.html          # Main application (single file, ~3000 lines)
├── README.md           # Documentation (this file)
├── LICENSE             # MIT License
├── CONTRIBUTING.md     # Contribution guidelines
├── CHANGELOG.md        # Version history
├── CODE_OF_CONDUCT.md  # Community guidelines
└── screenshots/        # Application screenshots
    ├── main-interface.png
    ├── statement-mode.png
    ├── syllogism-mode.png
    ├── euler-diagram.png
    ├── validity-check.png
    └── mobile-view.png

Performance
File Size: ~100KB (single HTML file)
Load Time: < 1 second on typical connections
Memory Usage: Minimal (no external resources)
Canvas Rendering: 60fps on modern devices
Accessibility
Keyboard navigable form controls
High contrast color options
Readable font sizes
Responsive layout for various screen sizes
🎓 Educational Background
The Six Validity Rules
A categorical syllogism is valid if and only if it satisfies all six of these rules:

Rule 1: Three Terms
A valid syllogism must contain exactly three terms, each used consistently with the same meaning throughout.

Violation: Fallacy of Four Terms (Quaternio Terminorum)

Rule 2: Middle Term Distribution
The middle term must be distributed (referring to all members of its category) in at least one premise.

Violation: Undistributed Middle

Rule 3: Conclusion Distribution
Any term distributed in the conclusion must also be distributed in its corresponding premise.

Violations:

Illicit Major (major term distributed in conclusion but not in major premise)
Illicit Minor (minor term distributed in conclusion but not in minor premise)
Rule 4: Exclusive Premises
A valid syllogism cannot have two negative premises.

Violation: Fallacy of Exclusive Premises

Rule 5: Negative Matches
If either premise is negative, the conclusion must be negative. If both premises are affirmative, the conclusion must be affirmative.

Violations:

Drawing affirmative conclusion from negative premise
Drawing negative conclusion from affirmative premises
Rule 6: Existential Rule
A particular conclusion cannot be drawn from two universal premises (in Boolean logic).

Violation: Existential Fallacy

Proposition Types
Type	Name	Standard Form	Subject Distribution	Predicate Distribution
A	Universal Affirmative	All S are P	Distributed	Undistributed
E	Universal Negative	No S are P	Distributed	Distributed
I	Particular Affirmative	Some S are P	Undistributed	Undistributed
O	Particular Negative	Some S are not P	Undistributed	Distributed
Distribution Explained
A term is distributed when the proposition makes a claim about all members of that category:

A (All S are P): S is distributed (we’re talking about ALL S), P is not (only some P may be S)
E (No S are P): both distributed (ALL S excluded from ALL P)
I (Some S are P): neither distributed (only SOME of each)
O (Some S are not P): P is distributed (excluded from the ENTIRE category P)
The Four Figures
The figure of a syllogism is determined by the position of the middle term (M):

Figure	Major Premise	Minor Premise	Memory Aid
1	M — P	S — M	M descends left side
2	P — M	S — M	M on the right
3	M — P	M — S	M on the left
4	P — M	M — S	M ascends left side
Boolean vs. Aristotelian Logic
Aspect	Boolean Logic	Aristotelian Logic
Empty Sets	Allowed	Not assumed
Universal Statements	No existential import	Imply existence
Valid Forms	15 forms	24 forms
“All S are P”	True if no S exist	Assumes S exist
📝 Citation
If you use Syllogiser in your research, teaching, or publications, please cite:

APA Format
Lam, W. I. (2026). Syllogiser: A Venn and Euler diagram tool for categorical logic [Computer software]. GitHub. https://github.com/jwilam/syllogiser

MLA Format
Lam, Wai Ip. Syllogiser: A Venn and Euler Diagram Tool for Categorical Logic. Version 30, 2026, github.com/jwilam/syllogiser.

Chicago Format
Lam, Wai Ip. “Syllogiser: A Venn and Euler Diagram Tool for Categorical Logic.” Computer software. GitHub, 2026. https://github.com/jwilam/syllogiser.

BibTeX
bibtex
@software{lam2026syllogiser,
  author    = {Lam, Wai Ip},
  title     = {Syllogiser: A Venn and Euler Diagram Tool for Categorical Logic},
  year      = {2026},
  version   = {30},
  publisher = {GitHub},
  url       = {https://github.com/jwilam/syllogiser},
  note      = {Interactive web application for visualizing categorical logic}
}

🤝 Contributing
Contributions are welcome and appreciated! Please read the guidelines below before contributing.

Ways to Contribute
Report Bugs: Open an issue describing the bug, steps to reproduce, and expected behavior
Suggest Features: Open an issue with the “enhancement” label
Improve Documentation: Fix typos, add examples, or clarify explanations
Submit Code: Fork, branch, code, test, and submit a pull request
Share: Tell others about Syllogiser, write tutorials, or create videos
Development Guidelines
Fork the repository

Create a branch for your feature:

bash
git checkout -b feature/amazing-feature

Make changes following the existing code style

Test thoroughly across multiple browsers

Commit with clear, descriptive messages

Push to your branch

Open a Pull Request with a detailed description

Code Style
Use 4 spaces for indentation
Comment complex logic
Keep functions focused and under 50 lines when possible
Use meaningful variable and function names
Test on Chrome, Firefox, and Safari at minimum
Reporting Issues
When reporting bugs, please include:

Browser name and version
Operating system
Steps to reproduce the issue
Expected behavior vs. actual behavior
Screenshots if applicable
Console errors if any
📄 License
This project is licensed under the MIT License.

text
MIT License

Copyright (c) 2026 LAM Wai Ip

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

👤 Author
LAM Wai Ip 林葦葉

Institution: The University of Hong Kong (HKU)
Faculty: Faculty of Education
Official Website: https://web.edu.hku.hk/faculty-academics/jwilam
Personal Website: https://jwilam.com
Email (Official): jwilam@hku.hk
Email (Personal): jwilam@gmail.com
Development Credits
Designer: LAM Wai Ip (HKU)
Developer: Claude-Opus 4.5 (Anthropic)
Version: 30
Release Date: February 14, 2026
☎️ Contact & Support
Getting Help
Documentation: Read this README and the built-in Help modal
Issues: GitHub Issues
Email: jwilam@hku.hk
Feedback
We welcome your feedback to improve Syllogiser! You can:

Open an issue on GitHub
Send an email with suggestions
Share your use cases and experiences
Support the Project
If you find Syllogiser useful:

Star the repository on GitHub
Share it with colleagues and students
Cite it in your publications
Report bugs and suggest improvements
Acknowledgments
Traditional logic textbooks and educators who inspired this project
The academic community for feedback and suggestions
Open source contributors and the web development community
