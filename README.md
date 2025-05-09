🐮 Copy-On-Write (COW) Vulnerability Lab (Dirty COW)

This repository contains my work on the Copy-On-Write (COW) vulnerability, commonly known as Dirty COW, based on the SEED Labs.

🔍 Vulnerability Overview
Dirty COW (CVE-2016-5195) is a privilege escalation vulnerability in the Linux kernel caused by a race condition in the memory management system's Copy-On-Write mechanism. This flaw allows an unprivileged local user to gain write access to read-only memory mappings, enabling them to modify files they should not have access to, including system binaries.

🧪 What I Learned
      How COW works in Linux and how the vulnerability exploits a race condition between madvise() and ptrace()/write().

      Writing and running a Dirty COW exploit to overwrite a protected system file.

      Mitigation techniques and understanding of kernel patches that fix the issue.
