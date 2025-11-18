# Plant Phenotyping Pipeline Website

This website presents the research paper "A Data-Driven Image Analysis Pipeline for Plant Phenotyping in Greenhouse Environments" in a format similar to the PRMI dataset website.

## Structure

```
website/
├── index.html          # Main HTML file
├── css/                # CSS framework files (Skeleton CSS)
│   ├── normalize.css
│   └── skeleton.css
├── js/                 # JavaScript files (if needed)
│   ├── jquery.min.js
│   └── footable.js
└── images/             # Image assets
    ├── greenhouse_system.png
    ├── pipeline_overview.png
    ├── dataset_summary.png
    ├── segmentation_results.png
    ├── feature_extraction.png
    ├── arxiv.jpg
    ├── dataset.png
    ├── code.png
    ├── logo.png
    └── webicon.jpg
```

## Required Images

You'll need to add the following images to the `images/` directory:

1. **greenhouse_system.png** - Image of the Texas A&M AgriLife Precision Automated Phenotyping Greenhouse system
2. **pipeline_overview.png** - Overview diagram of the image processing pipeline (from Figure 2 in your paper)
3. **dataset_summary.png** - Table or visualization showing the PGP v2 dataset summary
4. **segmentation_results.png** - Results showing segmentation performance (from Figure 3 in your paper)
5. **feature_extraction.png** - Visualization of feature extraction results (from Figure 5 in your paper)
6. **arxiv.jpg** - ArXiv logo (for paper link)
7. **dataset.png** - Dataset icon/logo
8. **code.png** - Code/GitHub icon
9. **logo.png** - Texas A&M or lab logo
10. **webicon.jpg** - Favicon for the website

## Customization

1. **Update Links**: Edit the links in the "Materials" section to point to your actual paper, dataset, and code repositories
2. **Add Images**: Replace placeholder image references with your actual figures from the paper
3. **Citation**: Update the citation section with the actual publication venue and year
4. **Authors**: Verify all author names and affiliations are correct

## Deployment

This is a static website that can be deployed to:
- GitHub Pages
- Any static hosting service
- Your institution's web server

Simply upload all files maintaining the directory structure.

## Based On

This website structure is based on the PRMI dataset website: https://gatorsense.github.io/PRMI/

