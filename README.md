# TYPO3 Extension `panopto`

Provides a content element for the integration of the end-to-end-video-content-management-system panopto.

## Usage

Install the extension and add the template include "Panopto".

## Content Element Options

You find a detailed description of each option for the panopto player here:
https://support.panopto.com/s/article/Embed-a-Video

## Configuration

the cType for this extension is `ce.panopto`

#### Panopto domain / path

there are typoscript constants for the panopto domain and path which can be easily overwritten.

```typo3_typoscript
PANOPTO {
  DOMAIN = https://demo.hosted.panopto.com/
  PATH = Panopto/Pages/
}
```

#### Template

you can also add your own template path if you

```typo3_typoscript
tt_content.ce\.panopto {
  templateRootPaths {
    30 = EXT:yourExtension/Resources/Private/Templates/
  }
}
```

## Requirements

* TYPO3 10.4 or newer
* PHP 7.2 or newer

## Screenshots

![Create Content Element wizard](Documentation/Images/createCe.png)
Fig. 1) Create Content Element wizard


![Panopto Content Element](Documentation/Images/ce.png)
Fig. 2) Panopto Content Element