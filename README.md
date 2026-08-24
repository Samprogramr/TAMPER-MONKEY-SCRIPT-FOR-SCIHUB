# Sci-Hub Paper Opener

A powerful Tampermonkey userscript that adds a custom right-click context menu to open academic papers directly through Sci-Hub. This tool streamlines the process of accessing research papers by automatically detecting DOIs and academic URLs, then constructing the appropriate Sci-Hub link.

![Version](https://img.shields.io/badge/version-3.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Platform](https://img.shields.io/badge/platform-All%20Browsers-orange)
![Made with Love](https://img.shields.io/badge/Made%20with-%E2%9D%A4-red)

## 📑 Table of Contents

- [Features](#-features)
- [Installation](#-installation)
- [Usage](#-usage)
- [Supported Websites](#-supported-websites)
- [Configuration](#-configuration)
- [FAQ](#-faq)
- [Troubleshooting](#-troubleshooting)
- [Contributing](#-contributing)
- [License](#-license)
- [Disclaimer](#-disclaimer)
- [Support](#-support)

## ✨ Features

- **Custom Right-Click Menu**: Adds a beautiful context menu when right-clicking on academic links
- **Automatic DOI Detection**: Recognizes DOIs in various formats (10.xxxx/xxxxx)
- **Multiple Sci-Hub Mirrors**: Support for multiple working Sci-Hub domains
- **Easy Mirror Switching**: Quick switch between different Sci-Hub mirrors
- **Copy Functions**: Copy Sci-Hub URL or original DOI with one click
- **Zero Configuration**: Works out of the box with default settings
- **Lightweight**: Minimal impact on page load times
- **Cross-Browser**: Works with Chrome, Firefox, Edge, and Safari

## 🚀 Installation

### Prerequisites

1. Install **Tampermonkey** extension for your browser:
   - [Chrome Web Store](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo)
   - [Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/)
   - [Microsoft Edge Add-ons](https://microsoftedge.microsoft.com/addons/detail/tampermonkey/iikmkjmpaadaobahmlepeloendndfphd)
   - [Safari (Mac App Store)](https://apps.apple.com/app/tampermonkey/id1482490089)

### Installation Steps

1. **Click the Tampermonkey icon** in your browser toolbar
2. **Select "Create a new script"**
3. **Delete the default template** code
4. **Copy and paste** the entire script from [`sci-hub-paper-opener.js`](sci-hub-paper-opener.js)
5. **Save** (Ctrl+S or Cmd+S)
6. **Verify** the script is enabled (check the Tampermonkey dashboard)

### Video Tutorial

*Coming soon!*

## 📖 Usage

### Method 1: Right-Click Context Menu

1. Navigate to any academic paper page or search results
2. **Right-click** on a DOI link or academic paper URL
3. Select from the custom menu:
   - **📚 Open with Sci-Hub** - Opens the paper using your primary Sci-Hub mirror
   - **🔄 Open with sci-hub.ren** - Opens using the alternative mirror
   - **📋 Copy Sci-Hub URL** - Copies the complete Sci-Hub link to clipboard
   - **🔗 Copy Original URL** - Copies just the DOI or paper URL

### Method 2: Selected Text

1. **Select** any DOI text (e.g., `10.1038/nature12373`)
2. **Right-click** on the selected text
3. Choose your preferred option from the context menu

### Examples

**Right-clicking on this DOI link:**

https://doi.org/10.1038/nature12373


**Will give you options to open:**

https://sci-hub.su/https://doi.org/10.1038/nature12373



## 🌐 Supported Websites

The script automatically detects and works with links from:

### Major Publishers
- Elsevier (ScienceDirect)
- Springer Nature
- Wiley Online Library
- Taylor & Francis
- SAGE Publications
- Oxford Academic (OUP)
- Cambridge University Press
- De Gruyter
- Emerald Publishing
- Karger Publishers
- IEEE Xplore
- ACM Digital Library

### Scientific Journals
- [Nature.com](https://www.nature.com)
- [Science.org](https://www.science.org)
- [PNAS](https://www.pnas.org)
- [Cell Press](https://www.cell.com)
- [The Lancet](https://www.thelancet.com)
- [NEJM](https://www.nejm.org)
- [BMJ](https://www.bmj.com)
- [JAMA Network](https://jamanetwork.com)
- [Royal Society Publishing](https://royalsocietypublishing.org)

### Open Access Platforms
- [PLOS](https://www.plos.org)
- [Frontiers](https://www.frontiersin.org)
- [MDPI](https://www.mdpi.com)
- [Hindawi](https://www.hindawi.com)
- [BioMed Central](https://www.biomedcentral.com)
- [arXiv](https://arxiv.org)

### Research Databases
- [PubMed](https://pubmed.ncbi.nlm.nih.gov)
- [NCBI](https://www.ncbi.nlm.nih.gov)
- [Google Scholar](https://scholar.google.com)
- [ResearchGate](https://www.researchgate.net)
- [Semantic Scholar](https://www.semanticscholar.org)
- [SSRN](https://www.ssrn.com)
- [JSTOR](https://www.jstor.org)

### DOI Resolvers
- doi.org links
- dx.doi.org links
- Any URL containing a DOI pattern (10.xxxx/xxxxx)

## ⚙️ Configuration

### Changing Sci-Hub Mirror

1. Click the **Tampermonkey icon** in your browser
2. Find **"Sci-Hub Paper Opener"** in the menu
3. Select **"⚙️ Change Sci-Hub URL"**
4. Enter the new Sci-Hub URL (e.g., `https://sci-hub.ren`)
5. Click **OK**

### Current Working Mirrors

| Domain | Status | Last Updated |
|--------|--------|--------------|
| `https://sci-hub.su` | ✅ Working | 2024 |
| `https://sci-hub.ren` | ✅ Working | 2024 |
| `https://sci-hub.se` | ⚠️ Alternative | 2024 |
| `https://sci-hub.st` | ⚠️ Alternative | 2024 |
| `https://sci-hub.ru` | ⚠️ Alternative | 2024 |

### Default Configuration

- **Default Mirror**: `https://sci-hub.su`
- **Alternative Mirror**: `https://sci-hub.ren`
- **Menu Position**: At cursor location
- **Open Behavior**: New tab

## ❓ FAQ

### General Questions

**Q: Is this legal?**
A: Sci-Hub operates in a legal gray area. While it provides access to research papers, many are copyrighted. Use this tool at your own discretion and respect intellectual property rights. Consider using legal alternatives like institutional access, interlibrary loans, or contacting authors directly.

**Q: Do I need Tampermonkey?**
A: Yes, this script requires Tampermonkey (or similar userscript manager like Greasemonkey or Violentmonkey) to run.

**Q: Does it work on mobile browsers?**
A: Tampermonkey is available on Firefox for Android and some mobile browsers. However, the right-click context menu may not work properly on touch devices.

**Q: Is this free to use?**
A: Yes, this script is completely free and open source under the MIT license.

### Technical Questions

**Q: Why isn't the context menu showing up?**
A: 
- Make sure Tampermonkey is enabled
- Verify the script is enabled in Tampermonkey dashboard
- Check that you're right-clicking on an actual DOI or academic link
- Try refreshing the page
- Clear browser cache if issues persist

**Q: The Sci-Hub link isn't working. What should I do?**
A: Sci-Hub domains change frequently. Use the Tampermonkey menu to update to a working mirror:
1. Click Tampermonkey icon
2. Find "Sci-Hub Paper Opener"
3. Select "Change Sci-Hub URL"
4. Enter a working mirror

**Q: Can I use this with a VPN?**
A: Yes, the script works with VPNs. Some Sci-Hub mirrors may be blocked in certain countries, so using a VPN might be necessary.

**Q: Does this work with all journals?**
A: The script works with any DOI or academic URL. However, Sci-Hub might not have access to very recent papers (usually less than 1-2 years old) or some obscure journals.

**Q: Will this slow down my browser?**
A: No, the script is very lightweight and only activates when you right-click on relevant links.

### Usage Questions

**Q: Can I open multiple papers at once?**
A: Yes, you can right-click and open multiple papers. Each will open in a new tab.

**Q: How do I copy the Sci-Hub URL without opening it?**
A: Right-click on the DOI/link and select "📋 Copy Sci-Hub URL" from the context menu.

**Q: Can I set my own custom Sci-Hub mirror?**
A: Yes! Use the "Change Sci-Hub URL" option in the Tampermonkey menu to set any mirror you prefer.

**Q: Does it work with Google Scholar?**
A: Yes, it works with Google Scholar links and any DOI links found on the page.

**Q: Can I use it on PubMed?**
A: Absolutely! It works perfectly with PubMed DOIs and links.

## 🔧 Troubleshooting

### Common Issues and Solutions

**Issue**: Script installed but nothing happens
**Solution**: 
- Check if Tampermonkey is enabled (icon should be colored)
- Verify script is enabled in dashboard
- Reload the page after installation
- Try disabling other scripts that might conflict

**Issue**: Context menu shows but options don't work
**Solution**:
- Check browser console (F12) for errors
- Ensure pop-up blocker isn't blocking new tabs
- Try clearing browser cache
- Disable other extensions temporarily

**Issue**: Getting "Fixed Store" message in Tampermonkey
**Solution**: This is normal Tampermonkey behavior. It's not an error and doesn't affect the script's functionality.

**Issue**: Sci-Hub page shows "Article not found"
**Solution**:
- The paper might be too recent (less than 1-2 years old)
- Try a different Sci-Hub mirror
- Check if the DOI is correct
- The paper might not be in Sci-Hub's database

**Issue**: Context menu appears on non-academic links
**Solution**: The script might be detecting false positives. Report the issue on GitHub with the specific URL.

**Issue**: Right-click menu doesn't appear on some websites
**Solution**: Some websites override right-click behavior. Try selecting the DOI text first, then right-click.

## 🛠️ Development

### File Structure


├── sci-hub-paper-opener.js # Main script file
├── README.md # Documentation
├── LICENSE # MIT License
└── CONTRIBUTING.md # Contribution guidelines


### Version History
- **v3.0** (Current): Added custom context menu with multiple options
- **v2.0**: Added floating button and keyboard shortcuts
- **v1.0**: Initial release with basic right-click functionality

### Built With
- [Tampermonkey](https://www.tampermonkey.net/) - Userscript manager
- JavaScript (ES6+)
- HTML5/CSS3

### Browser Compatibility
| Browser | Support | Version |
|---------|---------|---------|
| Chrome | ✅ Full Support | 88+ |
| Firefox | ✅ Full Support | 78+ |
| Edge | ✅ Full Support | 88+ |
| Safari | ⚠️ Partial | 14+ |
| Opera | ✅ Full Support | 74+ |

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### Guidelines
- Maintain code style consistency
- Add comments for complex logic
- Update documentation for new features
- Test thoroughly before submitting
- Follow [Conventional Commits](https://www.conventionalcommits.org/)

### Development Setup
1. Clone the repository
2. Create a new Tampermonkey script
3. Copy the development version
4. Make your changes
5. Test in browser
6. Submit PR

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
MIT License

Copyright (c) 2024 Sci-Hub Paper Opener Contributors

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



## ⚠️ Disclaimer

**Educational Purpose Only**: This tool is provided for educational purposes only. The developers are not responsible for any misuse or legal issues arising from its use. Users should:

- Respect copyright laws and intellectual property rights
- Use institutional access when available
- Consider legal alternatives for accessing research
- Understand that Sci-Hub's legal status varies by jurisdiction
- Use this tool responsibly and ethically

**Privacy**: The script doesn't collect any personal data. It only runs in your browser and makes requests to Sci-Hub directly.

**No Warranty**: This software is provided "as is" without warranty of any kind, express or implied.

## 🙏 Acknowledgments

- Thanks to the [Tampermonkey](https://www.tampermonkey.net/) team for their excellent userscript manager
- The academic community for pushing for open access
- All contributors who help maintain and improve this script
- The open-source community for their invaluable resources

## 📞 Support

- **Issues**: [Open an issue](https://github.com/yourusername/sci-hub-paper-opener/issues)
- **Suggestions**: [Create a feature request](https://github.com/yourusername/sci-hub-paper-opener/issues/new)
- **Questions**: Check the [FAQ](#-faq) section first
- **Discussions**: [Join the discussion](https://github.com/yourusername/sci-hub-paper-opener/discussions)

## 📊 Project Stats

![GitHub stars](https://img.shields.io/github/stars/yourusername/sci-hub-paper-opener)
![GitHub forks](https://img.shields.io/github/forks/yourusername/sci-hub-paper-opener)
![GitHub issues](https://img.shields.io/github/issues/yourusername/sci-hub-paper-opener)
![GitHub pull requests](https://img.shields.io/github/issues-pr/yourusername/sci-hub-paper-opener)

## 🔗 Related Projects

- [Tampermonkey](https://www.tampermonkey.net/) - Userscript manager
- [Open Access Button](https://openaccessbutton.org/) - Legal alternative for finding papers
- [Unpaywall](https://unpaywall.org/) - Find legal open access versions
- [CORE](https://core.ac.uk/) - Open access research papers

---

**Made with ❤️ for the research community**

*Remember to support open access initiatives and use this tool responsibly.*

*If this project helps you, consider giving it a ⭐ on GitHub!*


