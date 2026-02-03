source("renv/activate.R")

# Load project libraries automatically
local({
  packages <- c(
    "readxl",
    "dplyr",
    "ggplot2",
    "tidyr",
    "stringr",
    "janitor",
    "here",
    "workflowr"
  )
  
  invisible(sapply(packages, function(pkg) {
    if (!require(pkg, character.only = TRUE, quietly = TRUE)) {
      warning(paste("Failed to load package:", pkg))
    }
  }))
})
