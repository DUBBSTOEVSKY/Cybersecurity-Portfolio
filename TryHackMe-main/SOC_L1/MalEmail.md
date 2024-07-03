# TryHackMe Threat Intelligence Tools — Task 7 Scenario 1

## Scenario: SOC Analyst on Duty

You're on the frontlines as a SOC Analyst. Several suspicious emails have landed in your inbox from coworkers. It's time to dig into these emails and extract crucial details to triage the incidents.

## Task: Analyzing Email2.eml

Our mission: Use the tools from this module (or any reliable resources) to dissect Email2.eml and answer the pertinent questions.

### Extracting Threat Intelligence

First, we break down the email using the classic investigative approach: Who, What, Where, When, Why, and How. We'll dive into the email and extract every piece of intel we can before tackling the questions.

### Step-by-Step Analysis

#### Downloading and Opening the File

1. **Download the Data**: Grab the Email2.eml file via the blue "Download Task Files" button in the task.
2. **Navigate to Downloads**: Open your Downloads folder.
3. **Open with Text Editor**: Use your preferred text editor (VScode, Sublime, Notepad++). Right-click Email2.eml and select "Open with Code."

#### Examining the File

1. **Header Information**:
   - **Sender**: LeHuong-accounts@gmail.com
   - **Receiver**: chris.lyons@supercarcenterdetroit.com
   - **Date**: Thu, 14 Dec 2017 19:14:14 +0100

2. **Attachment Details**:
   - **Attachment Name**: Proforma Invoice P101092292891 TT slip pdf.rar.zip
   - **Encoded Malware**: Detected as base64 encoded.

3. **IP Addresses**:
   - **Sender’s IP**: 134.19.187.230
   - **Receiver’s IP**: 217.61.97.194

### Verifying Intel with Tools

#### Cisco Talos Intelligence

- **IP Lookup**: The sender's IP, located in the Netherlands, is marked as Neutral.

#### Phish Tool

- **File Upload**: Upload Email2.eml to Phish Tool.
- **Intel Breakdown**: Headers, plaintext email, and attachments are analyzed.
- **File Hashes**: Obtain SHA-256 hash for further analysis.

### Checking the File Hash

#### MalwareBazaar

- **Search for Hash**: No results found. Remember, always cross-check multiple sources.

#### VirusTotal

- **Hash Lookup**: The file is confirmed as malicious. Vital intel acquired!

### Revisiting Cisco Talos

- **File Reputation Lookup**: Confirms the file's malicious nature, reinforcing our findings from VirusTotal.

### Answering TryHackMe Questions

1. **Recipient’s Email Address**:
   - **Answer**: chris.lyons@supercarcenterdetroit.com

2. **Detection Alias from Talos Intelligence**:
   - **Answer**: HIDDENEXT/Worm.Gen

## Conclusion

This exercise demonstrates the power of methodical analysis and cross-referencing with multiple intel sources. Whether using Cisco Talos, Phish Tool, MalwareBazaar, or VirusTotal, always dig deep and verify your findings. Stay sharp and ahead of the threats.