<h1>Git Best Practices</h1>
<h2>Table of Contents</h2>
<ol>
<li>
        <a href="#atomic-commits">Atomic Commits</a>
</li>
<li>
        <a href="#conventional-commits">Conventional Commits</a>
</li>
<li>
        <a href="#atomic-vs-conventional">Atomic vs Conventional Commits</a>
</li>
<li>
        <a href="#references">Useful References</a>
</li>
</ol>
<hr>
<h2 id="atomic-commits">Atomic Commits</h2>
<h3>Motivation</h3>
<p>
The principle of atomicity, borrowed from the realm of databases, where transactions are indivisible units, serves as the bedrock for atomic commits in version control systems like Git. An atomic commit is designed to encapsulate a single logical change, ensuring that each commit is self-contained and can be understood, reviewed, and if necessary, reverted independently. This approach enhances the clarity and maintainability of the commit history, making it easier for developers to collaborate and manage changes in a codebase.
</p>
<h3>Example</h3>
<p>
Imagine you're working on a web application and you decide to implement a new "Contact Us" form, as well as fix a typo in the footer.
</p>
<p>
1. Identify Logical Units: The new form and the typo fix are unrelated changes. Thus, they should be committed separately.
</p>
<p>
2. Stage Changes Separately: Use <code>git add -p</code> to stage changes selectively. This command allows you to review and add changes hunk by hunk.
</p>
<li>
First, stage and commit the typo fix in the footer.
</li>
<li>
Next, stage the changes related to the "Contact Us" form.
</li>
<p>
3. Commit Each Change: For each staged change, use git commit with a descriptive message. For example:
</p>
<ul>
<li>
For the typo fix: <code>git commit -m "fix: correct typo in footer"</code>
</li>
<li>
For the new form: <code>git commit -m "feat: add contact us form"</code>
</li>
</ul>
<hr>
<h2 id="conventional-commits">Conventional Commits</h2>
<h3>Motivation</h3>
<p>
The conventional commit specification emerged from the need to standardize commit messages to make them more readable for humans and parsable by machines. This standardization supports automated tools in version management, changelog generation, and more, streamlining the release process and enhancing project communication.
</p>
<h3>Example</h3>
<p>
Suppose you're continuing to work on the web application, and now you need to add error handling to the "Contact Us" form.
</p>
<p>
1. Write a Conventional Commit Message: Following the conventional commit format, your commit message should include a type, scope, and description.
</p>
<ul>
<li>
Type: Could be feat, fix, docs, style, refactor, test, chore, etc.
</li>
<li>
Scope: Optional, indicates which part of the project is affected.
</li>
<li>
Description: A brief description of the change.
</li>
</ul>
<p>
2. Commit the Change: For adding error handling, your commit message might look like this:
</p>
<ul>
<li>
<code>git commit -m "feat(contact): add error handling to contact us form"</code>
</li>
<li>
This message clearly indicates the nature of the change, the area of the application it affects, and what specifically was done.>
</li>
</ul>
<hr>
<h2 id="atomic-vs-conventional">Atomic vs Conventional Commits</h2>
<p>
While atomic commits and conventional commits both aim to improve the clarity and utility of the commit history, they focus on different aspects of commit practices. Atomic commits prioritize the content and scope of changes, ensuring that each commit is limited to a single logical change. This practice makes the project history easier to navigate and understand on a granular level.
</p>
<p>
Conventional commits, on the other hand, standardize the format and semantics of commit messages. This structured approach facilitates automated processing for version management and changelog generation, enhancing project communication and streamlining the release process.
</p>
<p>
In essence, atomic commits improve the internal quality of the commit history, making it more manageable for developers, while conventional commits enhance the external communication and automation capabilities of the version control system. Together, they form a comprehensive approach to managing and documenting software development efforts effectively.>
</p>
<hr>
<h2 id="references">Useful Links and References</h2>
<ul>
    <li>
        <a href="https://en.wikipedia.org/wiki/Atomic_commit" target="_blank">Atomic Commits - Wikipedia</a>
    </li>
    <li>
        <a href="https://git-scm.com/book/en/v2" target="_blank">Git Pro Book</a>
    </li>
    <li>
        <a href="https://git-scm.com/docs/git-add" target="_blank">Git Documentation</a>
    </li>
    <li>
        <a href="https://www.conventionalcommits.org/en/v1.0.0/" target="_blank">Conventional Commits - Official Site</a>
    </li>
    <li>
        <a href="https://semantic-release.gitbook.io/semantic-release/" target="_blank">Semantic Release Documentation</a>
    </li>
</ul>
<hr>
