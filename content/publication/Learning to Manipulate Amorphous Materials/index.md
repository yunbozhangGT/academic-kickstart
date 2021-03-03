---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Learning to Manipulate Amorphous Materials"
authors: [Yunbo Zhang, Wenhao Yu, C. Karen Liu, Charles C.  Kemp, Greg Turk]
date: 2020-12-31
doi: ""

# Schedule page publish date (NOT publication's date).
# publishDate: 2019-09-13T14:19:20-04:00
# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "Transactions of Graphics (SIGGRAPH Asia), 2020"
publication_short: "SIGGRAPH Asia 2020"

abstract: "We present a method of training character manipulation of amorphous materials such as those often used in cooking.  Common examples of amorphous materials include granular materials (salt, uncooked rice), fluids (honey), and visco-plastic materials (sticky rice, softened butter).  A typical task is to spread a given material out across a flat surface using a tool such as a scraper or knife.  We use reinforcement learning to train our controllers to manipulate materials in various ways.   The training is performed in a physics simulator that uses position-based dynamics of particles to simulate the materials to be manipulated.  The neural network control policy is given observations of the material (e.g. a low-resolution density map), and the policy outputs actions such as rotating and translating the knife.  We demonstrate policies that have been successfully trained to carry out the following tasks: spreading, gathering, and flipping.  We produce a final animation by using inverse kinematics to guide a character's arm and hand to match the motion of the manipulation tool such as a knife or a frying pan."

# Summary. An optional shortened abstract.
summary: 

tags: []
categories: []
featured: true

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: 
url_code: 
url_dataset:
url_poster:
url_project:
url_slides:
url_source:
url_video: "https://www.youtube.com/watch?v=3fC6x2uxU9E"

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: "Smart"
  preview_only: true

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
