This repository contains annotated aortic centerlines and masks for 101 randomly selected images from [LIDC/IDRI](https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=1966254) and aortic centerlines for 41 randomly selected images from [AMOS](https://amos22.grand-challenge.org). Aortic centerlines were annotated by placing the knots on axial, sagittal, and coronal projections, while aortic masks were annotated on every third axial slice and linearly interpolated for the rest. 

The annotation was prepared for the paper [Robust Curve Detection in Volumetric Medical Imaging via Attraction Field].

We encourage the community to use the annotation to facilitate further advancements in the curves detection field.

# Annotation structure
## Directory
```
annotation
└─── amos
│   └─── knots
│       │   id1.json
│       │   id2.json
│       │   ...
└─── lidc
│   └─── knots
│       │   id1.json
│       │   id2.json
│       │   ...
│   └─── masks
│       │   id1.npy.gz
│       │   id2.npy.gz
│       │   ...
```
## Knots json

```
{
    'id': id
    'knots': [[x, y, z], ...]
}
```

# Usage

`example.ipynb` contains an example of matching the annotation with images from the dataset.

# Questions

If you have any questions please feel free to open an [issue](https://github.com/neuro-ml/curves-detection/issues).

# Cite


 
# License

The annotation is distributed according to the [Attribution-NonCommercial 4.0 International (CC BY-NC 4.0) (https://creativecommons.org/licenses/by-nc/4.0/), which means that you can freely use the data for any non-commercial purpose as long as you give appropriate credit to the authors.
