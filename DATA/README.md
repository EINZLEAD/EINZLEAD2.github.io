DATA folder

- Purpose: Store extracted images and text from exported backups created by the site.
- Usage: Place an exported backup file (the `.txt` you downloaded via "Export All") anywhere in your computer and run the included `import_backup.py` script to extract files into this `DATA/` folder.

Example:

```bash
python import_backup.py --input /path/to/lovelife-backup-2025-12-29.txt --outdir DATA
```

The script will create `DATA/images/`, `DATA/letters.json`, and `DATA/appreciation.html` (and save a copy of the original backup inside `DATA/`).

Note: This runs locally and modifies files in your repository/workspace only; the web app running in a browser cannot directly write into this folder.
