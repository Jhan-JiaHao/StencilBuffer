# StencilBuffer

![GitHub releases](https://github.com/Jhan-JiaHao/StencilBuffer/blob/main/Img/StencilBuffer_000.gif)

# Table of contents

<!--ts-->
  * [StencilBuffer](#stencilbuffer)
   >* [Installation](#installation)
   >* [Requirement](#requirement)
   >* [Usage](#usage)
   >* [Back](#back)
<!--te-->

## Installation

[![GitHub releases](https://img.shields.io/static/v1?style=for-the-badge&label=GitHub%20Releases&labelColor=181717&message=Downloads&color=green&logo=GitHub&logoColor=white)](https://github.com/Jhan-JiaHao/StencilBuffer/releases/tag/Stencil)

你可以使用以下方法安裝Stecil Effect
1.  __從[Releases Page](https://github.com/Jhan-JiaHao/StencilBuffer/releases/tag/Stencil)__ 在這裡您可以選擇以下選項：
* **StencilBuffer.unitypackage** - 這相當於您在資源商店中找到的內容，所有包含StencilBuffer的原始代碼都在這裡。
## Requirement
* Unity：URP 2022.3 up
## Usage

1.將下載下來的"StencilBuffer.unitypackage"導入至Unity專案，在Assets/Plugins/StencilBuffer路徑打開SampleScene
![GitHub releases](https://github.com/Jhan-JiaHao/StencilBuffer/blob/main/Img/StencilBuffer_001.png)
2.打開Edit/Project Settings，並確定其中的Quality/Rendering/Render Pipeline Asset指定為Assets/Settings/CustomSetting/URP-Stencil
![GitHub releases](https://github.com/Jhan-JiaHao/StencilBuffer/blob/main/Img/StencilBuffer_002.png)
3.以SampleScene為例，場景為一個立方體物件，其中四個面向的Plane只顯示特定物件的需求，我們需要針對四個面進行材質的相關設定

![GitHub releases](https://github.com/Jhan-JiaHao/StencilBuffer/blob/main/Img/StencilBuffer_003-1.gif)

![GitHub releases](https://github.com/Jhan-JiaHao/StencilBuffer/blob/main/Img/StencilBuffer_003-2.gif)

4.接著我們再依據想被特定面顯示的物件進行layer的設定

![GitHub releases](https://github.com/Jhan-JiaHao/StencilBuffer/blob/main/Img/StencilBuffer_004-1.gif)

![GitHub releases](https://github.com/Jhan-JiaHao/StencilBuffer/blob/main/Img/StencilBuffer_004-2.gif)

5.

## Back
* [GeneralAssets](https://github.com/Jhan-JiaHao/GeneralAssets)
# Maintainers
* [@Digispace](https://github.com/XRDigispace)
* [@Depstruct](https://github.com/Depstruct)
* [@JiaHao](https://github.com/Jhan-JiaHao)
