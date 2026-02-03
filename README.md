# HonorsThesis

A [workflowr][] project with [renv][] for package management.

[workflowr]: https://github.com/workflowr/workflowr
[renv]: https://rstudio.github.io/renv/

## Getting Started

### First Time Setup (New Machine)

1. **Open the project** in VS Code or RStudio
2. R will automatically activate the renv environment
3. **Install all required packages** by running in the R console:
   ```r
   renv::restore()
   ```
   This reads the `renv.lock` file and installs the exact package versions used in this project.

### Regular Workflow

Once set up, just open the project and everything loads automatically!

- **To build/view the website:** `wflow_build()` or `wflow_publish()`
- **After installing new packages:** Run `renv::snapshot()` to update the lockfile

## Project Structure

- `analysis/` - R Markdown source files for the website
- `docs/` - HTML output (rendered website)
- `code/` - R scripts
- `Data/` - Data files
- `output/` - Analysis outputs

## Troubleshooting

If packages aren't loading correctly:
```r
renv::restore()  # Reinstall packages from lockfile
```

If renv seems broken:
```r
renv::repair()   # Fix library issues
```
