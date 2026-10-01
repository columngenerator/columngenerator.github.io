# Column Generator (HTML, CSS, JavaScript)

A powerful, browser-based text parser that extracts, transforms, and exports structured data from raw text lines. Built entirely with HTML, CSS, and vanilla JavaScript — configure regex-powered column rules, apply replacements, map locations, and export to multiple formats including TXT, CSV, and DOCX. No frameworks or build tools required!

## 📊 Features

  * Customizable regex-powered column extraction rules 🔍
  * Multiple extraction types: regex, fixed values, and "between" delimiters 🎯
  * Post-processing options: last match, action mapping, frequency extraction, location mapping, time ranges, and case transforms ⚙️
  * Location name mapper with bulk import support 📍
  * Post-processing find & replace rules (literal or regex) 🔁
  * Additional pre-formatted data merging with source tracking 🛰️
  * Alternative text output using custom templates 📝
  * Sort output by date & time (ascending/descending) 🕐
  * Group output by action or source 🏷️
  * Time-based filtering (remove records before cutoff times) 🗑️
  * Export to **TXT**, **CSV**, and **DOCX** (both summary table and structured report formats) 📄
  * Live preview table with grouping separators 📋
  * Vertical and horizontal layout toggles 🔀
  * Auto-save state to local storage 💾
  * Responsive dark-themed design for desktop and mobile 📱

## 🚀 Getting Started

### Run Locally

1.  Clone this repository:

    ```bash
    git clone https://github.com/columngenerator/columngenerator.github.io
    ```

2.  Navigate to the project folder:

    ```bash
    cd columngenerator.github.io
    ```

3.  Open `index.html` in your browser.

That’s it! No build tools or server required.

## Online Demo

You can also use the application directly via GitHub Pages:
[https://columngenerator.github.io](https://columngenerator.github.io)

## 📁 Project Structure

```
index.html        # Main application (HTML, CSS & JS)
```

## 📖 How It Works

1.  **Paste raw text** into the input panel.
2.  **Configure column rules** — define how each column should be extracted using regex patterns, fixed values, or delimiters.
3.  **Add replacements & location mappings** to normalize your data.
4.  **(Optional) Add pre-formatted additional data** with a Source column that merges into your output.
5.  **Set options** — separator, sorting, grouping, default source label, and more.
6.  **Parse & Generate** — view the structured output in table and text formats.
7.  **Export** your results as TXT, CSV, or DOCX documents.

### Extraction Types

  * `regex` — Capture groups via regular expressions
  * `fixed` — Static/constant values
  * `between` — Text found between two delimiters

### Post-Processing Options

  * `lastMatch` — Use the last regex match
  * `actionMap` — Map action keywords (e.g. ПОДАВЛЕННЯ → ПРИДУШЕНО)
  * `freqExtract` — Extract frequency values from parentheses
  * `locationMap` — Apply configured location name mappings
  * `timeRange` — Preserve full time ranges
  * `uppercase` / `lowercase` / `trim` — Text transforms

## 💻 Technologies Used

  * **HTML5** for structure
  * **CSS3** for layout & dark-themed design
  * **JavaScript (ES6)** for parsing logic
  * **[docx](https://github.com/dolanmiu/docx)** (via CDN) for DOCX generation
  * **[FileSaver.js](https://github.com/eligrey/FileSaver.js)** (via CDN) for file downloads

## 📄 License

This project is released under the MIT License. Feel free to use, modify, and distribute.

## 🙏 Acknowledgments

Built to simplify the extraction and formatting of structured data from unstructured text records.
