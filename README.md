# SandboxEscaper
The sandbox escaper is a powerful tool that I have developed in C#. It consists of two files: a static class that holds data of other antimalware programs (AntiMalwareDataBase) and a static class that uses this database and performs the checks (SandBoxEscaper).

SandBoxEscaper is specifically designed to detect the presence of a sandbox environment that is often used to test malware. To achieve this, the tool performs various checks in a particular order. Firstly, it checks for VM resources by searching for known names of files that are typically used to create a virtual machine (VM) for testing malware.

Next, SandBoxEscaper performs a check on processes and services by searching for known names of those that are typically used in a sandbox environment. It also checks for a VM's BIOS ID, as VMs usually use an obfuscated BIOS ID that is distinct from a real computer's. Finally, the tool checks the manufacturer of the "PC" to see if it is identified with known sandbox conventions.

SandBoxEscaper's AntiMalwareDataBase is a database of many known antivirus, endpoint detection and response (EDR), and Windows Defender resources. The currently supported antivirus and EDR resources that it checks are: Eset, BitDefender, VGA, Norton, Sophos, TrendMicro, Avast, and McAfee. If there are any other vendors that users want to add, they can send an email to ilaysam00@gmail.com and I will add them to the AntiMalwareDataBase.

In summary, SandBoxEscaper is a highly efficient tool that can detect the presence of sandbox environments that are often used to test malware. Its AntiMalwareDataBase, containing a comprehensive list of antivirus, EDR, and Windows Defender resources, makes it one of the most reliable tools for detecting and bypassing sandbox environment
