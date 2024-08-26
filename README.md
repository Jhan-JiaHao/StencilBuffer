# StencilBuffer

![GitHub releases](https://github.com/Jhan-JiaHao/StencilBuffer/blob/main/Img/StencilBuffer_000.gif)

> StencilBuffer(模板)主要應用於改變被Assign物件的渲染狀態，最常見的用例是利用其效果屏蔽其他Shader的渲染顯示，使其只會顯示被Assign特定Layer的物件渲染顯示。

# Table of contents

<!--ts-->
  * [StencilBuffer](#stencilbuffer)
   >* [Installation](#installation)
   >* [Requirement](#requirement)
   >* [Usage](#usage)
   >* [Back To GeneralAssets](https://github.com/Jhan-JiaHao/GeneralAssets)
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

5.接著我們確認Assets/Settings/CustomSetting/URP-Stencil-Renderer的設定，Opaque Layer Mask及Transparent Layer Mask中，StencilLayer001-004皆不勾選(如圖所示)
![GitHub releases](https://github.com/Jhan-JiaHao/StencilBuffer/blob/main/Img/StencilBuffer_005-1.png)
![GitHub releases](https://github.com/Jhan-JiaHao/StencilBuffer/blob/main/Img/StencilBuffer_005-2.png)
6.最後我們確認Stencil 1 Opaque (Render Objects)、Stencil 2 Opaque (Render Objects)、Stencil 3 Opaque (Render Objects)、Stencil 4 Opaque (Render Objects)的相關設定
![GitHub releases](https://github.com/Jhan-JiaHao/StencilBuffer/blob/main/Img/StencilBuffer_006.png)
7.我們將設定依據紅框處設定即可(如圖)
![GitHub releases](https://github.com/Jhan-JiaHao/StencilBuffer/blob/main/Img/StencilBuffer_007.png)

8.其中需特別注意的是Stencil中的Value值，需對應我們Assign給顯示面的材質球ID(如圖)

![GitHub releases](https://github.com/Jhan-JiaHao/StencilBuffer/blob/main/Img/StencilBuffer_008.gif)

9.當我們將一切設定好，它就能順利運作

![GitHub releases](https://github.com/Jhan-JiaHao/StencilBuffer/blob/main/Img/StencilBuffer_000.gif)

10.我們也可以將其套用在其他應用上

![GitHub releases](https://github.com/Jhan-JiaHao/StencilBuffer/blob/main/Img/StencilBuffer_009.gif)

總結：
我們大致可以這樣簡單理解，將物件個別想像為"只顯示某物件的平面"和"只被某顯示平面顯示的物件"，我們將前者Assign帶有Stencil ID的材質球，並賦予其指定ID編號，後者我們將其利用物件的Layer和場景其他物件做渲染區隔，最後再利用Render Setting裡將兩者各自對應的Stencil ID和Layer綁定在一起，即可做到指定物件只會被指定的平面給予渲染出畫面。

最後祝一切順利，Enioy it! :)

## Back
* [Back To GeneralAssets](https://github.com/Jhan-JiaHao/GeneralAssets)
# Maintainers
* [@Digispace](https://github.com/XRDigispace)
* [@Depstruct](https://github.com/Depstruct)
* [@JiaHao](https://github.com/Jhan-JiaHao)
