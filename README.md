# GIS BSc — GIS als räumliches Denken in der Geographie

This repository contains a static web export of a German Bachelor-level GIS learning module. The material introduces GIS not only as software handling, but as a way of representing, managing, analysing and interpreting spatial information in geography.

Published course entry point:

<https://gisma-courses.github.io/gisbsc/index.html>

## Content overview

The course is organized into five learning units:

| Unit | Topic | Main focus |
|---|---|---|
| `GISBScL1` | GIS als räumliches Denken in der Geographie | Spatial thinking, geographic information, spatial concepts, coordinate systems, basic GIS orientation |
| `GISBScL2` | Relationen und Datenbanken | Data management, relational data models, attribute and geometry editing, spatial and relational queries |
| `GISBScL3` | Räumliche Analysemethoden | Spatial analysis, interpolation concepts, terrain analysis, derivation of spatial information from primary data |
| `GISBScL4` | Räumliche Entscheidungsfindung | Criteria, multi-criteria analysis, GIS-based decision support, project-oriented application |
| `GISBScL5` | Die Projektarbeit | Planning, structuring, implementing and presenting GIS project work |

The visible course logic combines conceptual GIS foundations with practical GIS workflows and a project-based final orientation.

## Repository structure

```text
.
├── index.html              # Central published entry page
├── GISBScL1/de/            # Unit 1: GIS and spatial thinking
├── GISBScL2/de/            # Unit 2: Relations and databases
├── GISBScL3/de/            # Unit 3: Spatial analysis methods
├── GISBScL4/de/            # Unit 4: Spatial decision-making
├── GISBScL5/de/            # Unit 5: Project work
├── core/                   # Shared static assets, scripts and styles
├── _templates/             # Legacy template material
├── daten/                  # Data files used by the course material
├── material/               # Additional course material
├── test/                   # Test or exercise-related material
├── .nojekyll               # Allows GitHub Pages to serve the static export unchanged
├── LICENSE                 # Repository-level CC0-1.0 license file
└── README.md
```

Most learning-unit folders contain static HTML pages plus associated `image`, `text`, and partly `multimedia` directories.

## How to use

The easiest way to use the course is through GitHub Pages:

<https://gisma-courses.github.io/gisbsc/index.html>

For local inspection, clone the repository and serve it as a static website:

```bash
git clone https://github.com/gisma-courses/gisbsc.git
cd gisbsc
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000/index.html
```

No build step is required. This repository is not structured as an active Quarto, R package, npm, or modern static-site-generator project. It is primarily a static course export.

## Technical character

The material appears to be a legacy eLearning export with pre-rendered HTML, CSS, JavaScript and generated navigation. The pages include references to eLML/GITTA-style course infrastructure and were designed as a self-contained web-based learning module.

For maintenance, the practical implication is simple: edit static HTML/assets directly, or migrate selected content into a modern teaching format such as Quarto, Markdown or a current learning-management system.

## Suitability

This repository is useful as:

- an archive of a complete German GIS introductory module,
- a source of conceptual GIS teaching material,
- a starting point for modernizing a GIS course,
- a structure reference for modular GIS teaching,
- raw material for extraction into a newer course website.

It is less suitable as:

- a directly maintainable modern course source,
- a current QGIS/R/GeoData workflow repository,
- a reproducible computational teaching project,
- a clean authoring repository with separated source and rendered output.

## Modernization notes

A practical modernization workflow would be:

1. Extract the conceptual text and learning objectives from the rendered HTML.
2. Rebuild the course structure in Quarto or another current authoring system.
3. Replace outdated software-specific exercises with current QGIS/R/geodata workflows.
4. Keep the five-unit didactic structure if the goal is a compact GIS foundation course.
5. Separate source material, rendered output, data and exercises more clearly.

## License note

The repository contains a `CC0-1.0` license file. Some legacy generated course pages may still display older embedded license or footer information from the original export. If the material is republished, remixed or redistributed outside this repository, the applicable license statement for the specific content should be checked explicitly.
