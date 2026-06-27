# Dataset

The datasets used in this work are hosted on Zenodo due to GitHub file size limitations.

## Download

Download all dataset files from the Zenodo record:

**DOI:** https://doi.org/...

Place the downloaded archives in this directory.

## Directory Structure

Place the downloaded archives in this directory:

```text
data/
├── corel5k_images.7z
├── scene_images.7z
└── ...
```

The notebooks will extract the archives automatically (if necessary) and use the extracted folders during execution.

After extraction, the directory should look like:

```text
data/
├── corel5k_images.7z
├── corel5k_images/
├── scene_images.7z
├── scene_images/
└── ...
```

## Notes

* Do not rename the downloaded files, as the notebooks expect the original filenames.
* If the datasets have already been extracted, the notebooks will skip the extraction step.
