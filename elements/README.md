## Circuit dataset reproduction files for CircuitExtractorYolo

Unfortunately due for copyright the dataset used by CircuitExtractorYolo cannot be made directly available, however this document and the files within this repo are intended do allow other to regenerate the same dataset from the same sources used in training of the original weights.

### How to use

The **source** directory contains the metadata files for the scientific publications that where used in [libscipaper's](https://github.com/IMbackK/libscipaper) metadata format. You will have to grab all of these pdfs, some, but not all, you will be able to grab using libscipaper's companion application [PdfGrabber](https://git-ce.rwth-aachen.de/carl_philipp.klemm/papergrabber)

The **location** directory contains the location of the Circuits on certain page in Yolo annotation format. The corresponding page is encoded into the filename with the schema being ${FILENAME}.pdf_${PAGENUMBER}P${CIRCUTYOLOCONFIDENCE}.txt
The pdfs corresponding to the **source** directory where exported using [poppler](https://poppler.freedesktop.org/) at 1280x1280 to create the images referred to in the **location** directory. The result-* files are special as they are unencumbered by copyright constraints, being exported from the schemata library underlying [RelaxIS](https://www.rhd-instruments.de/en/products/software/relaxis) these are thus supplied in this repo as is.

