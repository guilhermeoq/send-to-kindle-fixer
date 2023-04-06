
# Send to Kindle Fixer 📖

### About

When using the [Send to Kindle](https://www.amazon.com/sendtokindle) service to send .epub documents to your Kindle, you may encounter encoding issues in the file converted by Amazon. This happens because not every .epub file comes with the encoding information embedded. When this happens, Amazon assumes that the uploaded file is encoded with ISO-8859-1 and causes artifacts in the content, for example: â€œ.

This utility is available at Vercel: https://send-to-kindle-fixer.vercel.app

### Important
- Keep a copy of your original file: this utility may not be able to resolve the issue.
- This utility does not have access to your files. All processing takes place in your browser.

### What does this utility do?
- Fix UTF-8 encoding problem by adding UTF-8 declaration if no encoding is specified
- Fix hyperlink problem (result in Amazon rejecting the EPUB) when NCX table of content link to with ID hash.
- Detect invalid and/or missing language tag in metadata, and prompt user to select new language.
- Remove stray tags with no source field.

### What next?
Go to [Send to Kindle](https://www.amazon.com/sendtokindle) and check if the problem is resolved.
