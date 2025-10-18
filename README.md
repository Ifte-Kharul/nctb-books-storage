# NCTB Books Storage

This repository contains NCTB (National Curriculum and Textbook Board) books in PDF format, organized by class levels. For storage optimization, we use a hybrid approach:

- **Small/Medium Files**: Stored directly in this GitHub repository
- **Large Files**: Stored on Archive.org and linked through metadata

## Repository Structure

```
nctb-books-storage/
├── metadata/
│   ├── books.json        # Metadata for books stored in GitHub
│   └── large_files.json  # Metadata for books stored in Archive.org
├── pdfs/
│   ├── class1/
│   ├── class2/
│   └── ...
```

## File Storage Rules

- Files < 50MB: Stored directly in GitHub under appropriate class folders
- Files ≥ 50MB: Uploaded to Archive.org and referenced in `large_files.json`

## How to Use

1. Regular files can be accessed directly from their paths in the `pdfs` directory
2. For large files:
   - Check `metadata/large_files.json` for the Archive.org URL
   - Download directly from Archive.org using the provided link

## Contributing

1. For new books < 50MB:

   - Add the PDF to appropriate class folder
   - Update `metadata/books.json` with new entry

2. For new books ≥ 50MB:
   - Upload to Archive.org
   - Update `metadata/large_files.json` with new entry
