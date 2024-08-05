---
title: 'GreenFPGA: Evaluating FPGAs as Environmentally Sustainable Computing Solutions'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin
  - Aman Arora
  - Vidya A. Chhabria

# Author notes (optional)
#author_notes:
#  - 'Equal contribution'
#  - 'Equal contribution'

date: '2024-06-25T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
#publishDate: '2017-01-01T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference'] #Conference
#publication_types: ["article-journal"] #Journal 
#publication_types: ["article"] #Arxiv

# Publication name and optional abbreviated publication name.
publication: In *DAC 2024*
publication_short: In *DAC'24*

abstract: Growing global concerns about climate change highlight the need for environmentally sustainable computing. The ecological impact of computing, including operational and embodied, is a key consideration. Field Programmable Gate Arrays (FPGAs) stand out as promising sustainable computing platforms due to their reconfigurability across various applications. This paper introduces GreenFPGA, a tool estimating the total carbon footprint (CFP) of FPGAs over their lifespan, considering design, manufacturing, reconfigurability (reuse), operation, disposal, and recycling. Using GreenFPGA, the paper evaluates scenarios where the ecological benefits of FPGA reconfigurability outweigh operational and embodied carbon costs, positioning FPGAs as a environmentally sustainable choice for hardware acceleration compared to Application-Specific Integrated Circuits (ASICs). Experimental results show that FPGAs have lower CFP than ASICs, particularly for multiple distinct, low-volume applications, or short application lifespans.

# Summary. An optional shortened abstract.
summary: Tool to evaluate the carbon footprint of FPGA-based computing across its lifetime. The tool can also perform comparisons with ASIC counterpart considering differnt aspects such as manufacturing, recycling, disposal, reconfigurability (reuse), operation and design. The sustainable benifits of FPGA compared to ASIC is shown in this work.

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/abs/2311.12396'
url_code: 'https://github.com/ASU-VDA-Lab/GreenFPGA'
url_dataset: ''
url_poster: 'publication/greenfpga/greenfpga_dac24_poster.pdf'
url_project: ''
url_slides: 'publication/greenfpga/greenfpga_dac24_slides.pdf'
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: 'GreenFPGA'
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
#C projects:
#C   - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
#C slides: example
---


{{% callout note %}}
Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the _Slides_ button to check out the example.
{{% /callout %}}

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/).
