# OverTheWire Bandit – Linux Foundations for Cybersecurity

This repository documents my hands-on learning journey through the **OverTheWire Bandit wargame**. The goal is not to share solutions blindly, but to record **how I think, fail, research, and eventually understand Linux fundamentals** that are essential for cybersecurity.

> ⚠️ **Note**: Passwords are intentionally omitted. This repo focuses on concepts and learning outcomes, not spoilers.

---

## 🎯 Why Bandit?

Bandit is designed to teach Linux basics through practical challenges:

* File and directory navigation
* Permissions and ownership
* Searching and filtering data
* Working with encodings and binary files
* Thinking like an attacker: *"What is hidden here, and how can I extract it?"*

---

## 🧠 Learning Method

For every level, I document:

1. **Level Goal** – what the challenge asks
2. **What I Tried** – failed or incomplete attempts
3. **Key Commands** – tools involved (no passwords)
4. **Concept Learned** – the real takeaway

This helps me build **mental models**, not just memorize commands.

---

## 📘 Progress Summary

### Level 0 → 1: Getting Comfortable

**Concepts:**

* `ls`, `cat`
* Reading basic files

**Lesson:** Linux is literal. If you point to the right file, it will give you exactly what’s inside.

---

### Level 1 → 2: Special Filenames

**Concepts:**

* Filenames starting with `-`
* Input redirection `<`

**Lesson:** Some filenames conflict with command options. Redirection can bypass this.

---

### Level 2 → 3: Spaces & Quoting

**Concepts:**

* Quoting filenames with spaces
* Shell parsing

**Lesson:** Quoting is universal. It applies to *every* command, not just `cat`.

---

### Level 3 → 4: Hidden Files & Directories

**Concepts:**

* `ls -a`
* Hidden files
* Directories vs files

**Lesson:** Errors are informative. “Is a directory” tells you exactly what’s wrong.

---

### Level 4 → 5: Filenames Starting With `-`

**Concepts:**

* `--` (end of options)

**Lesson:** `--` forces the shell to treat everything after it as a filename, not an option.

---

### Level 5 → 6: Finding Files Precisely

**Concepts:**

* `find`
* File size (`-size`)
* File type (`-type f`)
* Executable flags

**Lesson:** Linux will find anything *if you describe it precisely enough*.

---

### Level 6 → 7: Ownership & Permissions

**Concepts:**

* `find /`
* `-user`, `-readable`, `-executable`

**Lesson:** Searching the entire filesystem requires accuracy and patience.

---

### Level 7 → 8: Searching Inside Files

**Concepts:**

* `grep`

**Lesson:** You don’t read large files manually. You ask Linux the right question.

---

### Level 8 → 9: Unique Data

**Concepts:**

* `sort`
* `uniq -u`
* Pipes `|`

**Lesson:** Many problems are solved by chaining small tools together.

---

### Level 9 → 10: Binary Files & Hidden Text

**Concepts:**

* Binary vs text files
* `strings`

**Lesson:** Binary files often contain readable information. Know how to extract it.

---

### Level 10 → 11: Encoding & Decoding

**Concepts:**

* Base64 encoding
* `base64 -d`

**Lesson:** Encoding and decoding are different operations. Tools do exactly what you tell them.

---

## 🛠️ Tools Practiced

* `ls`, `cd`, `cat`
* `find`
* `grep`
* `sort`, `uniq`
* `strings`
* `base64`


