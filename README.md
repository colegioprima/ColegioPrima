<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style> 
    .events-catcher,.window-events-catcher {
        left: 0;
        right: 0;
        bottom: 0;
        z-index: 2147483647;
        top: 0
    }
    
    .content-centered,.dialog-button-1 {
        text-align: center
    }
    
    .button,:focus {
        outline: 0
    }
    
    html,legend {
        color: #000
    }
    
    .no-wrap {
        white-space: nowrap
    }
    
    .white-space-normal {
        white-space: normal
    }
    
    .no-shadow {
        -moz-box-shadow: none;
        -webkit-box-shadow: none;
        box-shadow: none
    }
    
    .border-box-sizing {
        -ms-box-sizing: border-box;
        box-sizing: border-box;
        -moz-box-sizing: border-box;
        -webkit-box-sizing: border-box
    }
    
    .content-box-sizing {
        -ms-box-sizing: content-box;
        box-sizing: content-box;
        -moz-box-sizing: content-box;
        -webkit-box-sizing: content-box
    }
    
    .default-opacity-disabled.state-disabled {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=50)";
        filter: alpha(opacity=50);
        -moz-opacity: .5;
        -khtml-opacity: .5;
        opacity: .5;
        zoom:1}
    
    .opacity-0 {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=0)";
        filter: alpha(opacity=0);
        -moz-opacity: 0;
        -khtml-opacity: 0;
        opacity: 0;
        zoom:1}
    
    @media print {
        body {
            -webkit-print-color-adjust: exact
        }
    }
    
    body[contenteditable] {
        -webkit-user-modify: read-write;
        word-wrap: break-word;
        -webkit-nbsp-mode: space;
        -webkit-line-break: after-white-space
    }
    
    .templates-collection {
        display: none
    }
    
    .drop-panels-container {
        width: 10000px
    }
    
    .dialog-overlay {
        left: 0;
        top: 0;
        width: 100%;
        height: 100%;
        background: #555;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=80)";
        filter: alpha(opacity=80);
        -moz-opacity: .8;
        -khtml-opacity: .8;
        opacity: .8;
        zoom:1}
    
    .dir-ltr {
        direction: ltr
    }
    
    .dir-rtl {
        direction: rtl
    }
    
    .no-decorations {
        text-decoration: none!important
    }
    
    .transparent-text-box {
        background-color: transparent;
        border: none;
        padding: 0;
        margin: 0
    }
    
    .events-catcher,.events-catcher-background,.window-events-catcher {
        background: url(images/events-catcher-background.png)
    }
    
    .window-events-catcher {
        position: fixed
    }
    
    .events-catcher {
        position: absolute
    }
    
    .layer-1,.layer-2 {
        position: relative
    }
    
    .forwardLayerEvents {
        pointer-events: none
    }
    
    .catchLayerEvents {
        pointer-events: all!important
    }
    
    .testLayerForwarding {
        display: none!important
    }
    
    .text-overflow {
        white-space: nowrap;
        overflow: hidden;
        text-overflow: ellipsis
    }
    
    .hover-visible-items-container .hover-visible-item {
        display: none
    }
    
    .hover-visible-items-container:hover .hover-visible-item,.inline-block {
        display: inline-block
    }
    
    .opacity-icon {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=70)";
        filter: alpha(opacity=70);
        -moz-opacity: .7;
        -khtml-opacity: .7;
        opacity: .7;
        zoom:1}
    
    .opacity-icon:hover {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=90)";
        filter: alpha(opacity=90);
        -moz-opacity: .9;
        -khtml-opacity: .9;
        opacity: .9;
        zoom:1}
    
    .opacity-icon.state-pressed,.opacity-icon:active {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
        filter: alpha(opacity=100);
        -moz-opacity: 1;
        -khtml-opacity: 1;
        opacity: 1;
        zoom:1}
    
    .full-height {
        height: 100%
    }
    
    .full-width {
        width: 100%
    }
    
    .layer-1 {
        z-index: 1
    }
    
    .layer-2 {
        z-index: 2
    }
    
    .block,.left-block,.right-block {
        display: block
    }
    
    .uppercase-text {
        text-transform: UPPERCASE
    }
    
    .no-margin {
        margin: 0!important
    }
    
    .no-padding {
        padding: 0!important
    }
    
    .no-top-margin {
        margin-top: 0!important
    }
    
    .no-right-margin {
        margin-right: 0!important
    }
    
    .positioned-above {
        bottom: 100%;
        position: absolute
    }
    
    .positioned-beyond-left {
        right: 100%;
        position: absolute
    }
    
    .positioned-beyond-right {
        left: 100%;
        position: absolute
    }
    
    .positioned-right {
        right: 0;
        position: absolute
    }
    
    .positioned-top {
        position: absolute;
        top: 0
    }
    
    .positioned-bottom {
        position: absolute;
        bottom: 0
    }
    
    .positioned-below {
        top: 100%;
        position: absolute
    }
    
    .positioned-left {
        position: absolute;
        left: 0
    }
    
    .right-block {
        position: absolute;
        right: 0;
        top: 0;
        height: 100%
    }
    
    .left-block {
        position: absolute;
        left: 0;
        top: 0;
        height: 100%
    }
    
    .lower-case {
        text-transform: lowercase
    }
    
    .ignore-whitespace {
        font-size: 0
    }
    
    .vertically-scrollable {
        overflow-y: auto
    }
    
    .horizontally-scrollable {
        overflow-x: auto
    }
    
    .overflow-hidden,.scrollable-pane {
        overflow: hidden
    }
    
    .height-normalizer {
        height: 100%;
        width: 0;
        vertical-align: middle;
        display: inline-block
    }
    
    .float-left {
        float: left
    }
    
    .float-right {
        float: right
    }
    
    .float-clear {
        clear: both
    }
    
    .vertically-centered {
        vertical-align: middle;
        display: inline-block
    }
    
    .vertically-align-children:before,.vertically-bottom-children:before,.vertically-center-children:before,.vertically-top-children:before {
        content: "";
        height: 100%;
        width: 0;
        vertical-align: middle;
        display: inline-block
    }
    
    .vertically-center-children>* {
        vertical-align: middle;
        display: inline-block
    }
    
    .vertically-bottom-children>* {
        vertical-align: bottom;
        display: inline-block
    }
    
    .vertically-top,.vertically-top-children>* {
        vertical-align: top;
        display: inline-block
    }
    
    .vertically-bottom {
        vertical-align: bottom;
        display: inline-block
    }
    
    .content-left-align {
        text-align: left
    }
    
    .content-right-align {
        text-align: right
    }
    
    .wrap {
        white-space: normal
    }
    
    .positioned {
        position: relative
    }
    
    .absolute-positioned {
        position: absolute
    }
    
    .fixed-positioned {
        position: fixed!important
    }
    
    .top-most {
        z-index: 2147483647
    }
    
    .stretched-to-fill {
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0
    }
    
    .stretched-in-window {
        position: fixed;
        left: 0;
        top: 0;
        right: 0;
        bottom: 0
    }
    
    .stretch-vertically {
        position: absolute;
        bottom: 0;
        top: 0
    }
    
    .stretch-horizontally {
        position: absolute;
        left: 0;
        right: 0
    }
    
    .absolute-fill {
        position: absolute;
        width: 100%;
        height: 100%;
        top: 0;
        left: 0
    }
    
    .hidden {
        visibility: hidden
    }
    
    .instance-container.last-item .design-element.is-not-visible-in-last-data-item,.state-invisible,html.resume-editor.document-user-mode .design-element.last-section .design-element.is-not-visible-in-last-section,html.resume-viewer.document-user-mode .design-element.last-section .design-element.is-not-visible-in-last-section {
        visibility: hidden!important
    }
    
    .collapsed {
        display: none
    }
    
    .clear {
        clear: both
    }
    
    .selectable-text {
        cursor: text
    }
    
    .button {
        text-decoration: none
    }
    
    .button.custom-cursor.state-disabled {
        cursor: default
    }
    
    .button.custom-cursor.state-enabled {
        cursor: pointer
    }
    
    .state-hidden {
        display: none!important
    }
    
    .state-invisible {
        z-index: -1!important
    }
    
    textarea {
        resize: none;
        overflow: auto;
        white-space: pre-wrap
    }
    
    * {
        -webkit-tap-highlight-color: rgba(255,255,255,0)
    }
    
    .margin-bottom-3 {
        margin-bottom: 3px
    }
    
    .margin-right-5 {
        margin-right: 5px
    }
    
    .margin-right-15 {
        margin-right: 15px
    }
    
    .margin-right-10 {
        margin-right: 10px
    }
    
    .margin-right-20 {
        margin-right: 20px
    }
    
    .margin-left-25 {
        margin-left: 25px
    }
    
    .margin-left-5 {
        margin-left: 5px
    }
    
    .margin-left-10 {
        margin-left: 10px
    }
    
    .margin-top-10 {
        margin-top: 10px
    }
    
    .margin-left-0 {
        margin-left: 0
    }
    
    .margin-bottom-5 {
        margin-bottom: 5px
    }
    
    .margin-bottom-10 {
        margin-bottom: 10px
    }
    
    .shift-left-1 {
        margin-left: -1px
    }
    
    .padding-horizontal-20 {
        padding: 0 20px
    }
    
    .padding-horizontal-10 {
        padding: 0 10px
    }
    
    .padding-horizontal-5 {
        padding: 0 5px
    }
    
    .padding-vertical-10 {
        padding: 10px 0
    }
    
    .padding-vertical-5 {
        padding: 5px 0
    }
    
    .padding-10 {
        padding: 10px
    }
    
    .padding-5 {
        padding: 5px
    }
    
    .padding-top-10 {
        padding-top: 10px
    }
    
    .no-top-radius {
        -moz-border-radius-topleft: 0!important;
        -webkit-border-top-left-radius: 0!important;
        border-top-left-radius: 0!important;
        -moz-border-radius-topright: 0!important;
        -webkit-border-top-right-radius: 0!important;
        border-top-right-radius: 0!important
    }
    
    .no-bottom-radius {
        -moz-border-radius-bottomleft: 0!important;
        -webkit-border-bottom-left-radius: 0!important;
        border-bottom-left-radius: 0!important;
        -moz-border-radius-bottomright: 0!important;
        -webkit-border-bottom-right-radius: 0!important;
        border-bottom-right-radius: 0!important
    }
    
    .icon-size-10 {
        font-size: 10px!important
    }
    
    .icon-size-11 {
        font-size: 11px!important
    }
    
    .icon-size-12 {
        font-size: 12px!important
    }
    
    .icon-size-13 {
        font-size: 13px!important
    }
    
    .icon-size-14 {
        font-size: 14px!important
    }
    
    .icon-size-15 {
        font-size: 15px!important
    }
    
    .icon-size-16 {
        font-size: 16px!important
    }
    
    .icon-size-17 {
        font-size: 17px!important
    }
    
    .icon-size-18 {
        font-size: 18px!important
    }
    
    .icon-size-19 {
        font-size: 19px!important
    }
    
    .icon-size-20 {
        font-size: 20px!important
    }
    
    .icon-size-24 {
        font-size: 24px!important
    }
    
    .icon-size-32 {
        font-size: 32px!important
    }
    
    .cf:after,.cf:before {
        content: " ";
        display: table
    }
    
    .cf:after {
        clear: both
    }
    
    html {
        background: #FFF
    }
    
    blockquote,body,code,dd,div,dl,dt,fieldset,form,h1,h2,h3,h4,h5,h6,input,legend,li,ol,p,pre,td,textarea,th,ul {
        margin: 0;
        padding: 0
    }
    
    table {
        border-collapse: collapse;
        border-spacing: 0
    }
    
    fieldset,img {
        border: 0
    }
    
    address,caption,cite,code,dfn,th,var {
        font-style: inherit;
        font-weight: inherit
    }
    
    ol,ul {
        list-style: none
    }
    
    caption,th {
        text-align: left
    }
    
    h1,h2,h3,h4,h5,h6 {
        font-size: 100%;
        font-weight: 400
    }
    
    q:after,q:before {
        content: ''
    }
    
    abbr,acronym {
        border: 0;
        font-variant: normal
    }
    
    sup {
        vertical-align: text-top
    }
    
    sub {
        vertical-align: text-bottom
    }
    
    input,select,textarea {
        font-family: inherit;
        font-size: inherit;
        font-weight: inherit
    }
    
    .theme-extra-large-heading,.theme-large-heading,.theme-medium-heading,.theme-section-heading-small,.theme-small-heading {
        color: #2B2B2B;
        text-align: left
    }
    
    .cursor-n-resize {
        cursor: n-resize
    }
    
    .cursor-ne-resize {
        cursor: ne-resize
    }
    
    .cursor-nw-resize {
        cursor: nw-resize
    }
    
    .cursor-s-resize {
        cursor: s-resize
    }
    
    .cursor-se-resize {
        cursor: se-resize
    }
    
    .cursor-sw-resize {
        cursor: sw-resize
    }
    
    .cursor-w-resize {
        cursor: w-resize
    }
    
    .cursor-e-resize {
        cursor: e-resize
    }
    
    .cursor-move {
        cursor: move
    }
    
    .cursor-pointer {
        cursor: pointer
    }
    
    .cursor-default {
        cursor: default
    }
    
    .cursor-auto {
        cursor: auto
    }
    
    .cursor-not-allowed {
        cursor: not-allowed
    }
    
    .cursor-row-resize {
        cursor: row-resize
    }
    
    .cursor-ns-resize {
        cursor: ns-resize
    }
    
    .cursor-ew-resize {
        cursor: ew-resize
    }
    
    .loading-animation-dark-1 .loading-overlay {
        background: #373B43;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=45)";
        filter: alpha(opacity=45);
        -moz-opacity: .45;
        -khtml-opacity: .45;
        opacity: .45;
        zoom:1}
    
    .loading-animation-dark-1 .loading-animation {
        display: inline-block;
        width: 32px;
        height: 32px
    }
    
    html.wz-cssanimations .loading-animation-dark-1 .loading-animation {
        border: 5px solid rgba(255,255,255,.5);
        border-left-color: #fff;
        -moz-transform: translateZ(0);
        -webkit-transform: translateZ(0);
        -ms-transform: translateZ(0);
        transform: translateZ(0);
        -ms-transform: loadingAnimation 1s infinite linear;
        -webkit-animation: loadingAnimation 1s infinite linear;
        -moz-animation: loadingAnimation 1s infinite linear;
        animation: loadingAnimation 1s infinite linear;
        border-radius: 50%;
        -moz-border-radius: 50%;
        -webkit-border-radius: 50%;
        -ms-box-sizing: border-box;
        box-sizing: border-box;
        -moz-box-sizing: border-box;
        -webkit-box-sizing: border-box
    }
    
    html.wz-no-cssanimations .loading-animation-dark-1 .loading-animation {
        background-image: url(images/loading-animation-1.gif);
        background-position: center center;
        background-repeat: no-repeat
    }
    
    .icon-type-1 {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=80)";
        filter: alpha(opacity=80);
        -moz-opacity: .8;
        -khtml-opacity: .8;
        opacity: .8;
        zoom:1}
    
    .icon-type-1-container.state-selected .icon-type-1,.icon-type-1-container.state-toggled .icon-type-1,.icon-type-1-container:hover .icon-type-1 {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
        filter: alpha(opacity=100);
        -moz-opacity: 1;
        -khtml-opacity: 1;
        opacity: 1;
        zoom:1}
    
    .icon-type-2,.popup-scrollbar .scrollbar-handle {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=70)";
        -moz-opacity: .7;
        zoom:1}
    
    .icon-type-2 {
        filter: alpha(opacity=70);
        -khtml-opacity: .7;
        opacity: .7
    }
    
    .icon-type-2:hover {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=90)";
        filter: alpha(opacity=90);
        -moz-opacity: .9;
        -khtml-opacity: .9;
        opacity: .9;
        zoom:1}
    
    .icon-type-2.state-pressed,.icon-type-2:active {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
        filter: alpha(opacity=100);
        -moz-opacity: 1;
        -khtml-opacity: 1;
        opacity: 1;
        zoom:1}
    
    .theme-extra-large-heading {
        font-size: 40px;
        font-weight: 600
    }
    
    .theme-large-heading {
        font-size: 25px;
        font-weight: 400
    }
    
    .theme-medium-heading {
        font-size: 21px
    }
    
    .theme-small-heading {
        font-size: 18px;
        font-weight: 600
    }
    
    .theme-section-heading-small {
        font-size: 13px;
        font-weight: 600;
        line-height: 40px;
        height: 40px
    }
    
    .theme-section-heading-uppercase {
        color: #4a4f5b;
        font-size: 14px;
        text-transform: uppercase;
        font-weight: 600
    }
    
    .theme-text-link {
        color: #4297DC
    }
    
    .theme-text-link:hover {
        text-decoration: underline
    }
    
    .theme-text-button {
        color: #4297DC;
        text-decoration: none;
        font-size: 14px
    }
    
    .theme-text-button-small:hover,.theme-text-button:hover {
        text-decoration: underline
    }
    
    .theme-text-button-small {
        color: #4297DC;
        font-size: 13px
    }
    
    .theme-label,.theme-menu-item {
        text-decoration: none;
        font-weight: 600
    }
    
    .theme-paragraph-text {
        font-size: 14px;
        letter-spacing: 0;
        color: #8B8B8B;
        text-align: left
    }
    
    .theme-large-description {
        font-size: 14px;
        color: #2B2B2B;
        text-align: left
    }
    
    .theme-small-description {
        font-size: 12px;
        color: #6B6B6B;
        text-align: left
    }
    
    .theme-uppercase-sub-heading {
        font-size: 18px;
        font-weight: 600;
        color: #676767;
        text-transform: uppercase
    }
    
    .public-icons,.viewer-font-icon {
        font-style: normal;
        font-variant: normal;
        text-transform: none;
        line-height: 1;
        -moz-osx-font-smoothing: grayscale;
        -webkit-font-smoothing: antialiased
    }
    
    .theme-small-sub-heading {
        font-size: 15px;
        color: #676767;
        font-weight: 400
    }
    
    .theme-menu-item {
        font-size: 13px;
        color: #8B8B8B
    }
    
    .theme-field-label,.theme-label {
        font-size: 12px
    }
    
    .theme-menu-item:hover {
        color: #595959
    }
    
    .theme-label {
        color: #8B8B8B
    }
    
    .theme-window-title {
        font-size: 20px;
        font-weight: 600
    }
    
    .theme-colors-button-1 {
        color: #4a4f5b
    }
    
    .theme-colors-button-1.state-enabled:hover {
        color: #0288D1
    }
    
    .theme-colors-button-1.state-disabled {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=50)";
        filter: alpha(opacity=50);
        -moz-opacity: .5;
        -khtml-opacity: .5;
        opacity: .5;
        zoom:1}
    
    .theme-colors-button-4 {
        color: #4a4f5b
    }
    
    .theme-colors-button-4:hover {
        color: #777
    }
    
    .theme-colors-button-4.state-toggled {
        color: #303440
    }
    
    .theme-button-appearance-1 {
        color: #777981
    }
    
    .theme-button-appearance-1.state-enabled:hover {
        color: #617ab5
    }
    
    .theme-button-appearance-1.state-disabled {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=50)";
        filter: alpha(opacity=50);
        -moz-opacity: .5;
        -khtml-opacity: .5;
        opacity: .5;
        zoom:1}
    
    .loading-animations.layer-beneath-dialogs {
        z-index: 9999991
    }
    
    .loading-animations.layer-above-all {
        z-index: 2147483647
    }
    
    .loading-animations.layer-above-designer-pane {
        z-index: 99999
    }
    
    .loading-animations.layer-inline {
        z-index: 1
    }
    
    .element-overlays .element-overlay {
        opacity: .75;
        background: #000;
        z-index: -1
    }
    
    .element-overlays .overlay-content {
        width: 100%;
        color: #FFF
    }
    
    .element-overlays .overlay-content .overlay-icon {
        font-size: 50px
    }
    
    .element-overlays .overlay-content .overlay-message {
        padding: 10px;
        white-space: normal
    }
    
    .element-overlays .overlay-content .overlay-close {
        text-decoration: underline;
        cursor: pointer
    }
    
    .element-overlays.layer-beneath-dialogs {
        z-index: 9999991
    }
    
    .element-overlays.layer-above-all,.password-main {
        z-index: 2147483647
    }
    
    .element-overlays.layer-above-designer-pane {
        z-index: 99999
    }
    
    .element-overlays.layer-inline {
        z-index: 1
    }
    
    #freemium-footer,#freemium-footer-iframe-container,.drop-down-navigation.drop-panel-wrapper {
        z-index: 5000
    }
    
    .columns-grid {
        z-index: 5001
    }
    
    .marking-line,.ruler-grid-line {
        z-index: 99985
    }
    
    .add-section-button-decorator {
        z-index: 99986
    }
    
    .context-scroll-bar {
        z-index: 99987
    }
    
    .elements-decorator,.resize-grip.state-active,.resize-grip:hover {
        z-index: 99988
    }
    
    .resize-grip-icon {
        z-index: 99989
    }
    
    #control-box {
        z-index: 99990
    }
    
    .context-decorator,.element-resizable-handle,.element-resizing-handle {
        z-index: 99991
    }
    
    .designer-frame-decorator {
        z-index: 99993
    }
    
    .context-bar-panel,.context-toolbar-window {
        z-index: 99992
    }
    
    #bottom-designer-frame-decorators-container,#top-designer-frame-decorators-container,#vertical-ruler {
        z-index: 100000
    }
    
    #designer-page-header,#horizontal-ruler {
        z-index: 100001
    }
    
    #designer-footer,.context-container {
        z-index: 120000
    }
    
    #left-side-bars-container,#right-side-bars-container {
        z-index: 100012
    }
    
    #designer-header {
        z-index: 100013
    }
    
    #body-horizontal-scroller,#body-vertical-scroller {
        z-index: 100010
    }
    
    .design-tool {
        z-index: 1000000
    }
    
    .dialog,.dialog-overlay {
        z-index: 10000000
    }
    
    .callout,.ruler-coordinate-displayer,.tool-tip {
        z-index: 100000000
    }
    
    #notification-panel {
        z-index: 100000001
    }
    
    .ajax-operations-panel {
        z-index: 16776999
    }
    
    #offset-anchor {
        position: absolute;
        width: 0;
        top: 0;
        left: 50%
    }
    
    .loading-animation-1,.loading-animation-2 {
        width: 32px;
        display: inline-block;
        height: 32px
    }
    
    body.state-hierarchy-editing .design-element.root-instance {
        top: 0!important;
        left: 0!important;
        position: relative
    }
    
    .design-element h1,.design-element h2,.design-element h3 {
        display: inherit;
        font-size: inherit;
        margin: 0;
        font-weight: inherit
    }
    
    .transparent-background-small {
        background: url(images/transparent-background-small.png)
    }
    
    .transparent-background-2 {
        background: url(images/transparent-background-2.png)
    }
    
    .diagonal-red-background {
        background: url(images/diagonal-red.png) center center no-repeat
    }
    
    .horizontal-shadow-3 {
        position: absolute;
        left: 0;
        right: 0;
        height: 5px
    }
    
    .horizontal-shadow-3.bottom-to-top {
        background: url(images/horizontal-shadow-3-bottom-to-top.png) repeat-x
    }
    
    .horizontal-shadow-3.top-to-bottom {
        background: url(images/horizontal-shadow-3-top-to-bottom.png) repeat-x
    }
    
    .fully-transparent {
        background: url(images/fully-transparent.png)
    }
    
    .gradient-bottom-1 {
        background: url(images/gradient-bottom-1.png) left bottom repeat-x #fff
    }
    
    .animated-dash-red-white {
        background: url(images/animated-dash-red-white.gif)!important
    }
    
    .animated-dash-green {
        background: url(images/animated-dash-green.gif)!important
    }
    
    .animated-dashed-2 {
        background: url(images/animated-dashed-2.gif)
    }
    
    .checkers-texture-1 {
        background: url(images/checkers-texture-1.png)
    }
    
    .checkers-texture-2 {
        background: url(images/checkers-texture-2.png)
    }
    
    .diagonal-texture {
        background: url(images/texture-diagonal-black-on-transparent.png)
    }
    
    .spaced-dot-texture {
        background: url(images/spaced-dot.png)
    }
    
    .ui-autocomplete {
        max-height: 200px;
        overflow-y: auto;
        overflow-x: hidden
    }
    
    .ui-widget-content {
        border: 1px solid #ccc;
        background-color: #fff
    }
    
    .ui-widget-content a {
        color: #747171;
        font-weight: 400
    }
    
    .ui-widget-content a.ui-state-hover {
        color: #000;
        background: #e6e6e6;
        border: none;
        margin: 0!important;
        border-radius: 0;
        -moz-border-radius: 0;
        -webkit-border-radius: 0
    }
    
    .ui-widget-content a.state-pressed,.ui-widget-content a:active {
        background: #ddd
    }
    
    .loading-animation-1-background,html.wz-no-cssanimations .loading-animation-1,html.wz-no-cssanimations .loading-animation-2 {
        background-image: url(images/loading-animation-1.gif)
    }
    
    .loading-animation-1-background,.youtube-new-image-class,html.wz-no-cssanimations .loading-animation-1,html.wz-no-cssanimations .loading-animation-2 {
        background-position: center center;
        background-repeat: no-repeat
    }
    
    @font-face {
        font-family: viewer-font-icons;
        src: url(//webzaitest.blob.core.windows.net/assets/icons/201510261124216432/webzai-icons.eot);
        src: url(//webzaitest.blob.core.windows.net/assets/icons/201510261124216432/webzai-icons.eot#iefixhlochz) format('embedded-opentype'),url(//webzaitest.blob.core.windows.net/assets/icons/201510261124216432/webzai-icons.woff) format('woff'),url(//webzaitest.blob.core.windows.net/assets/icons/201510261124216432/webzai-icons.ttf) format('truetype'),url(//webzaitest.blob.core.windows.net/assets/icons/201510261124216432/webzai-icons.svg#font) format('svg');
        font-weight: 400;
        font-style: normal
    }
    
    .viewer-font-icon {
        font-family: viewer-font-icons;
        speak: none;
        font-weight: 400
    }
    
    .viewer-font-icon-popup-chevron-up:before {
        content: "\e904"
    }
    
    .viewer-font-icon-popup-chevron-down:before {
        content: "\e900"
    }
    
    .viewer-font-icon-popup-chevron-left:before {
        content: "\e901"
    }
    
    .viewer-font-icon-popup-chevron-right:before {
        content: "\e902"
    }
    
    .viewer-font-icon-popup-dots-horizontal:before {
        content: "\e903"
    }
    
    .viewer-font-icon-video-popup-next-video:before {
        content: "\e804"
    }
    
    .viewer-font-icon-video-popup-prev-video:before {
        content: "\e805"
    }
    
    .viewer-font-icon-video-popup-videos-list:before {
        content: "\e806"
    }
    
    .viewer-font-icon-popup-play-1:before {
        content: "\e801"
    }
    
    .viewer-font-icon-popup-play-2:before {
        content: "\e802"
    }
    
    .viewer-font-icon-popup-play-3:before {
        content: "\e803"
    }
    
    .viewer-font-icon-popup-nav:before {
        content: "\e800"
    }
    
    .viewer-font-icon-arrow_l:before {
        content: "\e60b"
    }
    
    .viewer-font-icon-arrow_r:before {
        content: "\e60c"
    }
    
    .viewer-font-icon-facebook:before {
        content: "\e60d"
    }
    
    .viewer-font-icon-google-plus:before {
        content: "\e60e"
    }
    
    .viewer-font-icon-link:before {
        content: "\e60f"
    }
    
    .viewer-font-icon-pinterest:before {
        content: "\e610"
    }
    
    .viewer-font-icon-polygon:before {
        content: "\e611"
    }
    
    .viewer-font-icon-slide-show-close-2:before {
        content: "\e612"
    }
    
    .viewer-font-icon-thumbnails:before {
        content: "\e613"
    }
    
    .viewer-font-icon-twitter:before {
        content: "\e614"
    }
    
    .viewer-font-icon-slide-show-dot-thumbnails:before {
        content: "\e60a"
    }
    
    .viewer-font-icon-angle-left:before {
        content: "\e605"
    }
    
    .viewer-font-icon-angle-right:before {
        content: "\e606"
    }
    
    .viewer-font-icon-slide-navigation-circle:before {
        content: "\e607"
    }
    
    .viewer-font-icon-slide-navigation-minus:before {
        content: "\e608"
    }
    
    .viewer-font-icon-slide-navigation-plus:before {
        content: "\e609"
    }
    
    .viewer-font-icon-button-menu:before {
        content: "\e600"
    }
    
    .viewer-font-icon-slide-navigation-close:before {
        content: "\e601"
    }
    
    .viewer-font-icon-slide-show-arrow-next:before {
        content: "\e603"
    }
    
    .viewer-font-icon-slide-show-arrow-prev:before {
        content: "\e604"
    }
    
    .viewer-font-icon-slide-show-close:before {
        content: "\e602"
    }
    
    @-moz-keyframes loadingAnimation {
        0% {
            -moz-transform: rotate(0);
            -webkit-transform: rotate(0);
            -ms-transform: rotate(0);
            transform: rotate(0)
        }
    
        100% {
            -moz-transform: rotate(360deg);
            -webkit-transform: rotate(360deg);
            -ms-transform: rotate(360deg);
            transform: rotate(360deg)
        }
    }
    
    @-ms-keyframes loadingAnimation {
        0% {
            -moz-transform: rotate(0);
            -webkit-transform: rotate(0);
            -ms-transform: rotate(0);
            transform: rotate(0)
        }
    
        100% {
            -moz-transform: rotate(360deg);
            -webkit-transform: rotate(360deg);
            -ms-transform: rotate(360deg);
            transform: rotate(360deg)
        }
    }
    
    @keyframes loadingAnimation {
        0% {
            -moz-transform: rotate(0);
            -webkit-transform: rotate(0);
            -ms-transform: rotate(0);
            transform: rotate(0)
        }
    
        100% {
            -moz-transform: rotate(360deg);
            -webkit-transform: rotate(360deg);
            -ms-transform: rotate(360deg);
            transform: rotate(360deg)
        }
    }
    
    html.wz-cssanimations .loading-animation-1,html.wz-cssanimations .loading-animation-2 {
        -ms-transform: translateZ(0);
        -webkit-animation: loadingAnimation 1s infinite linear;
        -moz-animation: loadingAnimation 1s infinite linear;
        -ms-box-sizing: border-box
    }
    
    html.wz-cssanimations .loading-animation-1 {
        border: 5px solid rgba(40,40,40,.2);
        border-left-color: #282828;
        -moz-transform: translateZ(0);
        -webkit-transform: translateZ(0);
        transform: translateZ(0);
        -ms-transform: loadingAnimation 1s infinite linear;
        animation: loadingAnimation 1s infinite linear;
        border-radius: 50%;
        -moz-border-radius: 50%;
        -webkit-border-radius: 50%;
        box-sizing: border-box;
        -moz-box-sizing: border-box;
        -webkit-box-sizing: border-box
    }
    
    html.wz-cssanimations .loading-animation-2 {
        border: 5px solid rgba(255,255,255,.4);
        border-left-color: #fff;
        -moz-transform: translateZ(0);
        -webkit-transform: translateZ(0);
        transform: translateZ(0);
        -ms-transform: loadingAnimation 1s infinite linear;
        animation: loadingAnimation 1s infinite linear;
        border-radius: 50%;
        -moz-border-radius: 50%;
        -webkit-border-radius: 50%;
        box-sizing: border-box;
        -moz-box-sizing: border-box;
        -webkit-box-sizing: border-box
    }
    
    @font-face {
        font-family: public-font-icons;
        src: url(//webzaitest.blob.core.windows.net/assets/icons/201610060849567328/webzai-icons.eot);
        src: url(//webzaitest.blob.core.windows.net/assets/icons/201610060849567328/webzai-icons.eot#iefixhlochz) format('embedded-opentype'),url(//webzaitest.blob.core.windows.net/assets/icons/201610060849567328/webzai-icons.woff) format('woff'),url(//webzaitest.blob.core.windows.net/assets/icons/201610060849567328/webzai-icons.ttf) format('truetype'),url(//webzaitest.blob.core.windows.net/assets/icons/201610060849567328/webzai-icons.svg#font) format('svg');
        font-weight: 400;
        font-style: normal
    }
    
    .youtube-new-image-class {
        background-image: url(images/yt_icon_rgb.png);
        max-width: 80%;
        height: 100%;
        width: 100%;
        margin-top: 0!important;
        top: 0!important;
        background-size: contain;
        margin: 0 auto
    }
    
    .public-icons {
        font-family: public-font-icons;
        speak: none;
        font-weight: 400
    }
    
    .scrollbar .scrollbar-body,.scrollbar .slide-area {
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0
    }
    
    .scrollbar .scrollbar-handle {
        background: #fff
    }
    
    .scrollbar.vertical {
        width: 10px
    }
    
    .scrollbar.vertical .scrollbar-handle {
        left: 0;
        right: 0
    }
    
    .scrollbar.horizontal {
        height: 10px
    }
    
    .scrollbar.horizontal .scrollbar-handle {
        top: 0;
        bottom: 0
    }
    
    .ui-effects-transfer {
        margin: 1px;
        border: 1px dashed #000;
        z-index: 200000
    }
    
    .ui-effects-explode,.ui-effects-wrapper {
        z-index: 2
    }
    
    .ui-slider .ui-slider-handle,.ui-slider .ui-slider-range {
        z-index: auto
    }
    
    .slide-scrollbar.vertical {
        position: absolute;
        display: block;
        right: 2px;
        top: 2px;
        bottom: 2px;
        width: 8px;
        border: none
    }
    
    .slide-scrollbar.vertical .scrollbar-handle {
        left: 0;
        right: 0;
        background: #bbb;
        border-radius: 2px;
        -moz-border-radius: 2px;
        -webkit-border-radius: 2px
    }
    
    .slide-scrollbar .slide-area {
        cursor: pointer;
        border-radius: 2px;
        -moz-border-radius: 2px;
        -webkit-border-radius: 2px
    }
    
    .slide-scrollbar.state-active .slide-area,.slide-scrollbar:hover .slide-area {
        background: #ddd
    }
    
    .slide-scrollbar.state-active .scrollbar-handle,.slide-scrollbar:hover .scrollbar-handle {
        background: #aaa
    }
    
    .dialog-button-1 {
        border-radius: 4px;
        -moz-border-radius: 4px;
        -webkit-border-radius: 4px;
        display: inline-block
    }
    
    .dialog-button-1.state-disabled {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=60)";
        filter: alpha(opacity=60);
        -moz-opacity: .6;
        -khtml-opacity: .6;
        opacity: .6;
        zoom:1}
    
    .dialog-button-1.variation-action {
        background: #0288D1;
        color: #fff;
        border: 1px solid #0288D1;
        box-shadow: 0 3px 0 #0288D1,0 6px 4px -2px rgba(0,0,0,.3);
        font-weight: 800
    }
    
    .dialog-button-1.variation-action.state-enabled:hover {
        background: #0298ea;
        border: 1px solid #0298ea;
        box-shadow: 0 3px 0 #0288D1,0 6px 4px -2px rgba(0,0,0,.3)
    }
    
    .dialog-button-1.variation-action.state-enabled.state-pressed,.dialog-button-1.variation-action.state-enabled:active {
        background: #02679e;
        border: 1px solid #02679e;
        box-shadow: 0 3px 0 #0288D1,0 6px 4px -2px rgba(0,0,0,.3)
    }
    
    .dialog-button-1.variation-secondary {
        background: #DEDEDE;
        color: #707070;
        border: 1px solid #cbcbcb;
        box-shadow: 0 3px 0 #AAA,0 6px 4px -2px rgba(0,0,0,.3);
        font-weight: 800
    }
    
    .dialog-button-1.variation-secondary.state-enabled:hover {
        background: #e6e6e6;
        border: 1px solid #d6d6d6
    }
    
    .dialog-button-1.variation-secondary.state-enabled.state-pressed,.dialog-button-1.variation-secondary.state-enabled:active {
        background: #d0d0d0;
        border: 1px solid silver
    }
    
    .dialog-button-1.variation-small {
        font-size: 14px;
        line-height: 28px;
        height: 28px;
        padding: 0 10px;
        min-width: 60px
    }
    
    .dialog-button-1.variation-medium {
        font-size: 16px;
        line-height: 38px;
        height: 38px;
        padding: 0 10px;
        min-width: 115px
    }
    
    .dialog-button-1.variation-large {
        font-size: 20px;
        line-height: 48px;
        height: 48px;
        padding: 0 10px;
        min-width: 125px
    }
    
    .dialog-button-1.variation-wide-small {
        font-size: 14px;
        line-height: 28px;
        height: 28px;
        padding: 0 15px;
        min-width: 105px;
        -ms-box-sizing: border-box;
        box-sizing: border-box;
        -moz-box-sizing: border-box;
        -webkit-box-sizing: border-box
    }
    
    .dialog-button-1.variation-wide-medium {
        font-size: 16px;
        line-height: 34px;
        height: 34px;
        padding: 0 10px;
        min-width: 150px;
        -ms-box-sizing: border-box;
        box-sizing: border-box;
        -moz-box-sizing: border-box;
        -webkit-box-sizing: border-box
    }
    
    .dialog-button-1.variation-wide-large {
        min-width: 200px;
        -ms-box-sizing: border-box;
        box-sizing: border-box;
        -moz-box-sizing: border-box;
        -webkit-box-sizing: border-box
    }
    
    .dialog-button-1.variation-block {
        display: block;
        padding: 0!important
    }
    
    .common-rich-content-style {
        white-space: pre-line;
        word-wrap: break-word
    }
    
    .common-rich-content-style ol,.common-rich-content-style ul {
        list-style-position: outside;
        padding: 0 .3em 0 2em;
        margin: 0;
        clear: both
    }
    
    .common-rich-content-style ol ol,.common-rich-content-style ol ul,.common-rich-content-style ul ol,.common-rich-content-style ul ul {
        padding: 0 2em
    }
    
    .common-rich-content-style.dir-rtl ol,.common-rich-content-style.dir-rtl ul {
        padding-left: 0!important
    }
    
    .common-rich-content-style.dir-ltr ol,.common-rich-content-style.dir-ltr ul {
        padding-right: 0!important
    }
    
    .common-rich-content-style p {
        margin: 0
    }
    
    .common-rich-content-style ul {
        list-style-type: disc
    }
    
    .common-rich-content-style ol {
        list-style-type: decimal
    }
    
    .common-rich-content-style.has-content:after {
        content: "";
        clear: both;
        display: block
    }
    
    .image-box-image-new.unknown-size,.image-box-image-wrapper.use-background-image .image-box-background-image,.image-box-image-wrapper.use-background-image .image-box-image-new,.image-box-image-wrapper.use-image-element.non-tile-layout .image-box-background-image,.image-box-image-wrapper.use-image-element.tile-layout .image-box-image-new {
        display: none!important
    }
    
    .common-rich-content-style.no-content:after {
        content: "\00a0"
    }
    
    body.scrolling-mode-touch .scrollable-pane {
        overflow: auto
    }
    
    .body-element-wrapper.slide-effect-body-wrapper {
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0
    }
    
    .slide-effect-body-container {
        position: relative;
        overflow: hidden
    }
    
    #body-element.slide-effect,.slide-effect-animation,.slide-effect-element-wrapper {
        position: absolute;
        left: 0;
        right: 0
    }
    
    .slide-effect-animation {
        top: 0;
        bottom: 0
    }
    
    .pc-desktop-mode .slide-effect-designer-pane {
        padding: 0!important
    }
    
    .slide-effect-events-catcher-layer {
        z-index: 99985
    }
    
    .slide-effect-element-wrapper {
        z-index: 99986;
        top: 0;
        bottom: 0
    }
    
    .image-box-new.state-image-error .image-box-image-new {
        width: 100%!important;
        height: 100%!important;
        margin: 0!important
    }
    
    .image-box-image-wrapper {
        overflow: hidden;
        background-repeat: no-repeat;
        text-align: left;
        position: relative
    }
    
    .image-box-image-wrapper.background-fixed {
        background-attachment: fixed
    }
    
    .image-box-image-wrapper.repeat,.image-box-image-wrapper.repeat .image-box-background-image {
        background-repeat: repeat
    }
    
    .image-box-image-wrapper.repeatVertically,.image-box-image-wrapper.repeatVertically .image-box-background-image {
        background-repeat: repeat-y
    }
    
    .image-box-image-wrapper.repeatHorizontally,.image-box-image-wrapper.repeatHorizontally .image-box-background-image {
        background-repeat: repeat-x
    }
    
    .image-box-image-wrapper.horizontal-center.vertical-top,.image-box-image-wrapper.horizontal-center.vertical-top .image-box-background-image {
        background-position: center top
    }
    
    .image-box-image-wrapper.horizontal-left.vertical-top,.image-box-image-wrapper.horizontal-left.vertical-top .image-box-background-image {
        background-position: left top
    }
    
    .image-box-image-wrapper.horizontal-right.vertical-top,.image-box-image-wrapper.horizontal-right.vertical-top .image-box-background-image {
        background-position: right top
    }
    
    .image-box-image-wrapper.horizontal-center.vertical-center,.image-box-image-wrapper.horizontal-center.vertical-center .image-box-background-image {
        background-position: center center
    }
    
    .image-box-image-wrapper.horizontal-left.vertical-center,.image-box-image-wrapper.horizontal-left.vertical-center .image-box-background-image {
        background-position: left center
    }
    
    .image-box-image-wrapper.horizontal-right.vertical-center,.image-box-image-wrapper.horizontal-right.vertical-center .image-box-background-image {
        background-position: right center
    }
    
    .image-box-image-wrapper.horizontal-center.vertical-bottom,.image-box-image-wrapper.horizontal-center.vertical-bottom .image-box-background-image {
        background-position: center bottom
    }
    
    .image-box-image-wrapper.horizontal-left.vertical-bottom,.image-box-image-wrapper.horizontal-left.vertical-bottom .image-box-background-image {
        background-position: left bottom
    }
    
    .image-box-image-wrapper.horizontal-right.vertical-bottom,.image-box-image-wrapper.horizontal-right.vertical-bottom .image-box-background-image {
        background-position: right bottom
    }
    
    .slideshow-thumbs-container .slideshow-thumbs-content,.slideshow-thumbs-container .thumbs .thumb {
        display: inline-block;
        height: 100%
    }
    
    .image-box-image-new {
        border: none!important
    }
    
    .image-box-image-wrapper.use-background-image.unknown-size {
        background: 0 0!important
    }
    
    .slideshow-thumbs-container .carousel-item {
        position: absolute;
        width: 100%;
        height: 100%
    }
    
    .slideshow-thumbs-container {
        position: relative;
        overflow: hidden;
        width: 100%;
        height: 100%
    }
    
    .slideshow-thumbs-container .thumbs {
        position: relative;
        left: 0;
        top: 0;
        height: 100%;
        white-space: nowrap
    }
    
    .popup-overlay-container {
        position: absolute;
        left: 0;
        top: 0;
        right: 0;
        bottom: 0;
        overflow: hidden;
        z-index: 100000
    }
    
    .popup-overlay-container .popup-background {
        position: absolute;
        left: 0;
        top: 0;
        right: 0;
        bottom: 0;
        background: rgba(0,0,0,.7);
        opacity: .8
    }
    
    .popup-overlay-container .popup-wrapper {
        position: absolute;
        left: 0;
        top: 0;
        width: 100%;
        height: 100%
    }
    
    .popup-overlay {
        position: absolute;
        width: 100%;
        height: 100%;
        text-align: left
    }
    
    .popup-overlay .close-button {
        position: absolute;
        z-index: 10
    }
    
    .popup-overlay .popup-header {
        height: 10%
    }
    
    .popup-overlay .slideshow-container {
        position: absolute;
        left: 0;
        right: 0
    }
    
    .popup-overlay .slideshow-container .carousel-container {
        height: 100%
    }
    
    .popup-overlay .slideshow-container .carousel-container .slideshow-carousel-container {
        height: 100%;
        overflow: hidden
    }
    
    .popup-overlay .slideshow-container .carousel-container .carousel-items {
        position: relative;
        height: 100%
    }
    
    .popup-overlay .slideshow-container .carousel-item {
        display: none;
        position: absolute;
        width: 100%;
        height: 100%;
        left: 0;
        top: 0
    }
    
    .popup-overlay .slideshow-container .carousel-item .image {
        position: absolute
    }
    
    .popup-overlay .slideshow-container .carousel-item .image img {
        display: inline-block;
        width: auto;
        height: auto;
        max-width: 100%;
        max-height: 100%
    }
    
    .popup-overlay .slideshow-container .carousel-item .video {
        position: absolute
    }
    
    .popup-overlay .slideshow-container .carousel-item .video img {
        display: inline-block;
        width: 100%;
        height: 100%
    }
    
    .popup-overlay .slideshow-container .carousel-item .video .video-container {
        position: absolute;
        width: 100%;
        height: 100%;
        left: 0;
        top: 0;
        cursor: pointer
    }
    
    .popup-overlay .slideshow-container .carousel-item .video .video-container .play-button {
        display: none;
        position: absolute;
        top: 50%;
        left: 50%;
        text-align: center
    }
    
    .popup-overlay .slideshow-container .carousel-item .video .video-container .play-button:before {
        display: inline-block
    }
    
    .popup-overlay .slideshow-container .carousel-item .video .video-container iframe {
        display: none;
        width: 100%;
        height: 100%
    }
    
    .popup-overlay .slideshow-container .carousel-item .video .video-container.ie8 iframe {
        display: block
    }
    
    .popup-overlay .slideshow-container .carousel-item .video .video-container.playing {
        z-index: 2
    }
    
    .popup-overlay .slideshow-container .carousel-item .video .video-container.playing .play-button {
        display: none
    }
    
    .popup-overlay .slideshow-container .carousel-item .video .video-container.playing iframe,.popup-overlay .slideshow-container .carousel-item.current .video .video-container .play-button {
        display: block
    }
    
    .popup-overlay .slideshow-container .carousel-item.current .video .video-container.playing .play-button,.popup-overlay .slideshow-container .carousel-item.state-loading .video .video-container .play-button {
        display: none
    }
    
    .popup-overlay .slideshow-container .navigation-button {
        position: absolute;
        z-index: 10
    }
    
    .popup-overlay .footer {
        position: absolute;
        left: 0;
        right: 0;
        bottom: 0
    }
    
    .popup-overlay .footer .thumbs-container {
        text-align: center
    }
    
    .popup-overlay .footer .thumbs-container .slideshow-thumbs-container {
        display: inline-block;
        width: auto;
        max-width: 100%
    }
    
    .popup-overlay .footer .thumbs-container .thumb .image-thumb {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=50)";
        filter: alpha(opacity=50);
        -moz-opacity: .5;
        -khtml-opacity: .5;
        opacity: .5;
        zoom:1}
    
    .popup-overlay .footer .thumbs-container .thumb .image-thumb:hover {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
        filter: alpha(opacity=100);
        -moz-opacity: 1;
        -khtml-opacity: 1;
        opacity: 1;
        zoom:1}
    
    .popup-overlay .footer .thumbs-container .thumb .image-thumb img {
        height: 100%
    }
    
    .popup-overlay .footer .thumbs-container .thumb.current .image-thumb {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
        filter: alpha(opacity=100);
        -moz-opacity: 1;
        -khtml-opacity: 1;
        opacity: 1;
        zoom:1}
    
    .popup-loading-animation .loading-overlay {
        background: url(images/events-catcher-background.png)
    }
    
    .popup-loading-animation .loading-animation {
        box-shadow: 0 0 2px rgba(0,0,0,.2);
        display: inline-block;
        width: 50px;
        height: 50px
    }
    
    .popup-overlay.single-item-popup .slideshow-container .navigation-button,.popup-overlay.single-item-popup .slideshow-container .numbers-container,.popup-overlay.video-popup .share-link.pinterest {
        display: none
    }
    
    html.wz-cssanimations .popup-loading-animation .loading-animation {
        border: 5px solid rgba(255,255,255,.4);
        border-left-color: #fff;
        -moz-transform: translateZ(0);
        -webkit-transform: translateZ(0);
        -ms-transform: translateZ(0);
        transform: translateZ(0);
        -ms-transform: loadingAnimation 1s infinite linear;
        -webkit-animation: loadingAnimation 1s infinite linear;
        -moz-animation: loadingAnimation 1s infinite linear;
        animation: loadingAnimation 1s infinite linear;
        border-radius: 50%;
        -moz-border-radius: 50%;
        -webkit-border-radius: 50%;
        -ms-box-sizing: border-box;
        box-sizing: border-box;
        -moz-box-sizing: border-box;
        -webkit-box-sizing: border-box
    }
    
    html.wz-no-cssanimations .popup-loading-animation .loading-animation {
        background-image: url(images/loading-animation-1.gif);
        background-position: center center;
        background-repeat: no-repeat
    }
    
    .explorer-mode .popup-overlay .image,.explorer-mode .popup-overlay .video-container,.explorer-mode .popup-overlay.popup-3 .slideshow-container .navigation-button {
        background: url(images/events-catcher-background.png)
    }
    
    .popup-overlay.single-item-popup .slideshow-container .carousel-item .no-title.no-description.no-link .image-text {
        height: auto
    }
    
    .popup-scrollbar {
        position: absolute;
        display: block;
        overflow: hidden;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=30)";
        filter: alpha(opacity=30);
        -moz-opacity: .3;
        -khtml-opacity: .3;
        opacity: .3;
        zoom:1;border-radius: 2px;
        -moz-border-radius: 2px;
        -webkit-border-radius: 2px
    }
    
    .popup-scrollbar:hover {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=60)";
        filter: alpha(opacity=60);
        -moz-opacity: .6;
        -khtml-opacity: .6;
        opacity: .6;
        zoom:1}
    
    .popup-scrollbar.vertical {
        width: 8px;
        right: 0;
        top: 0;
        bottom: 0
    }
    
    .popup-scrollbar .slide-area {
        cursor: pointer;
        border-radius: 2px;
        -moz-border-radius: 2px;
        -webkit-border-radius: 2px
    }
    
    .popup-scrollbar .scrollbar-handle {
        left: 0;
        right: 0;
        filter: alpha(opacity=70);
        -khtml-opacity: .7;
        opacity: .7;
        border-radius: 2px;
        -moz-border-radius: 2px;
        -webkit-border-radius: 2px
    }
    
    .dialog-mode-parents {
        height: 100%;
        -ms-box-sizing: border-box;
        box-sizing: border-box;
        -moz-box-sizing: border-box;
        -webkit-box-sizing: border-box
    }
    
    .dialog-mode-container {
        overflow: hidden!important;
        height: 100%
    }
    
    .parallax-image-active {
        overflow: hidden
    }
    
    html {
        width: 100%;
        height: 100%;
        padding: 0;
        margin: 0;
        -webkit-touch-callout: none;
        -webkit-user-select: none;
        -khtml-user-select: none;
        -moz-user-select: none;
        -ms-user-select: none;
        user-select: none
    }
    
    html .content-editable,html .has-rich-content,html .has-text,html .selectable-text {
        -webkit-touch-callout: text;
        -webkit-user-select: text;
        -khtml-user-select: text;
        -moz-user-select: text;
        -ms-user-select: text;
        user-select: text
    }
    
    .ck-object-container,.password-button,.store-selected-filters-element .filter-label,body.view-mode .webzai-clickable-behaviour {
        -ms-user-select: none;
        -webkit-user-select: none
    }
    
    html body.design-mode .has-rich-content,html body.design-mode .has-text {
        -webkit-touch-callout: none;
        -webkit-user-select: none;
        -khtml-user-select: none;
        -moz-user-select: none;
        -ms-user-select: none;
        user-select: none
    }
    
    html body {
        padding: 0;
        margin: 0;
        font-size: 13px;
        text-rendering: optimizeLegibility;
        -webkit-font-smoothing: antialiased
    }
    
    html body.design-mode.inner-screen-view {
        cursor: default
    }
    
    html body.view-mode {
        overflow-y: scroll!important;
        overflow-x: auto
    }
    
    html body.site-viewer {
        font-family: Arial,Helvetica,sans-serif
    }
    
    html body.site-viewer.mobile-client #body-element {
        position: relative;
        min-height: 0;
        left: auto;
        top: auto
    }
    
    html #body-element {
        height: auto;
        text-align: left
    }
    
    .layout-fill-horizontally {
        left: 0;
        width: 100%
    }
    
    .layout-fill-vertically {
        top: 0;
        height: 100%
    }
    
    body.loading-page * {
        cursor: progress!important
    }
    
    body.pc.full-screen-view.design-mode #body-element {
        width: auto!important
    }
    
    .design-element .cell-element.last {
        margin-right: 0!important
    }
    
    .design-element .row-element.desc-row.last,.design-element.last-section .row-element.root-row.last {
        margin-bottom: 0!important
    }
    
    .mobile-drop-area-marking {
        position: absolute;
        z-index: 99996
    }
    
    .mobile-drop-area-marking .marking-line {
        background: #323539
    }
    
    .mobile-drop-area-marking.row-area-marking .marking-main-line {
        top: 50%;
        height: 4px;
        margin-top: -2px
    }
    
    .mobile-drop-area-marking.row-area-marking .marking-left-line,.mobile-drop-area-marking.row-area-marking .marking-right-line {
        width: 4px
    }
    
    .mobile-drop-area-marking.column-area-marking .marking-main-line {
        left: 50%;
        width: 4px;
        margin-left: -2px
    }
    
    .mobile-drop-area-marking.column-area-marking .marking-left-line,.mobile-drop-area-marking.column-area-marking .marking-right-line {
        height: 4px
    }
    
    .mobile-dragging-helper-class {
        position: absolute!important;
        z-index: 99995;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=70)";
        filter: alpha(opacity=70);
        -moz-opacity: .7;
        -khtml-opacity: .7;
        opacity: .7;
        zoom:1}
    
    .cell-resizing-handle {
        width: 0;
        z-index: 99995
    }
    
    .cell-resizing-handle .marking-main-line {
        width: 2px;
        left: 50%;
        margin-left: -1px
    }
    
    .cell-resizing-handle .handle-inner-decorator {
        position: absolute;
        top: 50%;
        left: 50%;
        width: 8px;
        height: 24px;
        margin-left: -4px;
        margin-top: -12px;
        border-radius: 3px;
        -moz-border-radius: 3px;
        -webkit-border-radius: 3px;
        -ms-box-sizing: content-box;
        box-sizing: content-box;
        -moz-box-sizing: content-box;
        -webkit-box-sizing: content-box
    }
    
    .cell-resizing-handle .handle-inner-decorator,.cell-resizing-handle .marking-main-line {
        background: #25272B
    }
    
    .cell-resizing-handle:hover .handle-inner-decorator,.cell-resizing-handle:hover .marking-main-line {
        background: #323539
    }
    
    .cell-resizing-handle.state-active .handle-inner-decorator,.cell-resizing-handle.state-active .marking-main-line {
        background: #eba52b
    }
    
    .resume-built-by-section-element {
        font-size: 25px
    }
    
    .resume-built-by-section-element .resume-content-container {
        height: 100px;
        text-align: center
    }
    
    .resume-built-by-section-element .resume-content-container .label {
        color: silver;
        text-transform: uppercase;
        margin-right: 10px;
        font-size: 13px;
        font-weight: 600;
        line-height: 1
    }
    
    .ck-object-container {
        text-align: center;
        padding: 10px;
        clear: both;
        line-height: 0;
        -webkit-touch-callout: none;
        -khtml-user-select: none;
        -moz-user-select: none;
        user-select: none;
        -ms-box-sizing: border-box;
        box-sizing: border-box;
        -moz-box-sizing: border-box;
        -webkit-box-sizing: border-box
    }
    
    .ck-object-container.ck-object-layout-block {
        width: 100%!important
    }
    
    .ck-object-container.ck-object-align-left {
        text-align: left
    }
    
    .ck-object-container.ck-object-align-right {
        text-align: right
    }
    
    .ck-object-container.ck-object-layout-left {
        float: left
    }
    
    .ck-object-container.ck-object-layout-right {
        float: right
    }
    
    .ck-object-container.ck-object-layout-left .ck-object-wrapper,.ck-object-container.ck-object-layout-right .ck-object-wrapper {
        width: 100%!important
    }
    
    .ck-object-container.ck-object-layout-block .ck-object-wrapper,.ck-object-container.ck-object-layout-left .ck-object-wrapper,.ck-object-container.ck-object-layout-right .ck-object-wrapper {
        display: inline-block
    }
    
    .ck-object-container .ck-ratio *,.ckeditor-root-element .rich-content-video-iframe {
        display: none
    }
    
    .ck-object-container .ck-ratio {
        line-height: 0
    }
    
    .ck-object {
        width: 100%
    }
    
    .ck-object-wrapper {
        position: relative
    }
    
    .ck-object-image img,.ck-object-wrapper.lock-ratio .ck-object {
        position: absolute;
        left: 0;
        top: 0
    }
    
    .ck-object-video.ck-object-wrapper.lock-ratio .ck-object {
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0
    }
    
    .ckeditor-root-element .ck-object-hr .ck-object-wrapper {
        padding: 15px 0
    }
    
    .ckeditor-root-element .ck-object-hr hr {
        margin: 0 auto
    }
    
    .strikeout {
        font-size: 4em;
        line-height: 1em;
        position: relative
    }
    
    body.mobile-desktop-mode .slide-navigation-panel-2 .close-icon-content,body.mobile-desktop-mode .slide-navigation-panel-3 .close-icon-content {
        font-size: 20px
    }
    
    .strikeout::after {
        border-bottom: .125em solid #494F5B;
        content: "";
        left: 30%;
        margin-top: calc(-.0625em);
        position: absolute;
        right: 30%;
        top: 50%
    }
    
    .design-element.animation-hidden {
        display: none!important
    }
    
    .slide-navigation-panel-2 {
        height: 100%;
        position: relative;
        text-align: left
    }
    
    .slide-navigation-panel-2 .close-icon-content {
        position: absolute;
        top: 15px;
        right: 15px;
        font-size: 14px;
        cursor: pointer
    }
    
    .slide-navigation-panel-2 .side-bar {
        position: absolute;
        top: 0;
        bottom: 0;
        left: 0;
        width: 45px
    }
    
    .slide-navigation-panel-2 .page-item {
        position: relative
    }
    
    .slide-navigation-panel-2 .page-item.has-hierarchy .hierarchy-box,.slide-navigation-panel-2 .page-item:hover .hierarchy-box .hierarchy-separator,.slide-navigation-panel-2 .page-item:hover .hierarchy-box:hover .hierarchy-hover-overlay,.slide-navigation-panel-2 .page-item:hover .hover-overlay {
        display: block
    }
    
    .slide-navigation-panel-2 .page-title {
        padding-left: 10px;
        padding-right: 30px;
        text-transform: uppercase
    }
    
    .drop-down-navigation-desktop-panel .sub-hierarchy-icon,.drop-down-navigation-desktop-panel.sub-hierarchy-left .sub-hierarchy-icon {
        font-style: normal;
        font-variant: normal;
        text-transform: none;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        line-height: 1
    }
    
    .slide-navigation-panel-2 .title-container {
        position: relative;
        margin-left: 45px;
        margin-right: 50px;
        cursor: pointer
    }
    
    .slide-navigation-panel-2 .hierarchy-box {
        position: absolute;
        top: 0;
        bottom: 0;
        right: 0;
        width: 45px;
        display: none;
        text-align: center;
        cursor: pointer
    }
    
    .slide-navigation-panel-2 .hierarchy-separator {
        position: absolute;
        top: 8px;
        bottom: 8px;
        left: 0;
        width: 1px;
        display: none
    }
    
    .slide-navigation-panel-2 .hierarchy-icon {
        position: relative
    }
    
    .slide-navigation-panel-2 .hierarchy-hover-overlay {
        display: none
    }
    
    .slide-navigation-panel-2 .header {
        height: 80px;
        overflow: hidden;
        position: relative
    }
    
    .slide-navigation-panel-2.level-0>.panel-content .back {
        display: none
    }
    
    .slide-navigation-panel-2 .back {
        position: relative;
        padding-left: 75px;
        padding-right: 60px
    }
    
    .slide-navigation-panel-2 .back:hover .hover-overlay {
        display: block
    }
    
    .slide-navigation-panel-2 .panel-content {
        border-right: 1px solid
    }
    
    .slide-navigation-panel-2 .back-container {
        padding-top: 15px;
        padding-bottom: 15px;
        cursor: pointer;
        position: relative
    }
    
    .slide-navigation-panel-2 .back-title {
        margin-left: 10px
    }
    
    .slide-navigation-panel-2 .scrolling-pane,.slide-navigation-panel-2 .scrolling-view {
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0
    }
    
    .slide-navigation-panel-2 .scrolling-view {
        top: 80px;
        bottom: 20px
    }
    
    .slide-navigation-panel-2.color-negative .hover-overlay {
        background: #000
    }
    
    .slide-navigation-panel-2 .hover-overlay {
        background: #fff;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=10)";
        filter: alpha(opacity=10);
        -moz-opacity: .1;
        -khtml-opacity: .1;
        opacity: .1;
        zoom:1;display: none
    }
    
    .slide-navigation-panel-2 .panel-container {
        display: none
    }
    
    .slide-navigation-panel-2 a {
        color: inherit
    }
    
    .slide-navigation-panel-2 .panel-overlay {
        background-color: #000;
        opacity: 0;
        display: none
    }
    
    .slide-navigation-panel-2.during-animation .panel-overlay {
        display: block
    }
    
    .slide-navigation-panel-2.during-animation .panel-container {
        overflow: hidden
    }
    
    .slide-navigation-panel-2.in-animation>.panel-content .slide-scrollbar {
        visibility: hidden
    }
    
    .slide-navigation-panel-2.sub-panel-opened>.panel-content .slide-scrollbar {
        display: none
    }
    
    .slide-navigation-panel-2.sub-panel-opened>.panel-container {
        display: block
    }
    
    .slide-navigation-panel-2 .slide-scrollbar {
        right: -12px
    }
    
    .drop-down-navigation-desktop-panel>.content-container {
        position: relative
    }
    
    .drop-down-navigation-desktop-panel .border-box {
        border-style: solid
    }
    
    .drop-down-navigation-desktop-panel .pages-list {
        position: relative;
        -ms-box-sizing: border-box;
        box-sizing: border-box;
        -moz-box-sizing: border-box;
        -webkit-box-sizing: border-box
    }
    
    .drop-down-navigation-desktop-panel .page-content {
        position: relative
    }
    
    .drop-down-navigation-desktop-panel .page-item.simple .page-content {
        overflow: hidden;
        -ms-box-sizing: border-box;
        box-sizing: border-box;
        -moz-box-sizing: border-box;
        -webkit-box-sizing: border-box;
        cursor: pointer;
        padding-left: 20px;
        padding-right: 20px;
        height: 100%
    }
    
    .drop-down-navigation-desktop-panel .page-item {
        -ms-box-sizing: border-box;
        box-sizing: border-box;
        -moz-box-sizing: border-box;
        -webkit-box-sizing: border-box
    }
    
    .drop-down-navigation-desktop-panel.sub-hierarchy-left .sub-hierarchy-icon {
        font-size: inherit;
        font-family: viewer-font-icons;
        speak: none;
        font-weight: 400
    }
    
    .drop-down-navigation-desktop-panel.sub-hierarchy-left .sub-hierarchy-icon:before {
        content: "\e605"
    }
    
    .drop-down-navigation-desktop-panel.sub-hierarchy-left .sub-hierarchy-icon-container {
        right: auto;
        left: 0
    }
    
    .drop-down-navigation-desktop-panel.show-arrow .page-item.has-hierarchy>.item-block .sub-hierarchy-icon-container {
        display: inline-block
    }
    
    .drop-down-navigation-desktop-panel.show-arrow .page-item.has-hierarchy.simple .page-content {
        padding-right: 30px
    }
    
    .drop-down-navigation-desktop-panel.sub-hierarchy-left.show-arrow .page-item.has-hierarchy.simple .page-content {
        padding-right: 20px;
        padding-left: 30px
    }
    
    .drop-down-navigation-desktop-panel .sub-hierarchy-icon {
        font-size: inherit;
        font-family: viewer-font-icons;
        speak: none;
        font-weight: 400
    }
    
    .drop-down-navigation-desktop-panel .sub-hierarchy-icon:before {
        content: "\e606"
    }
    
    .drop-down-navigation-desktop-panel .sub-hierarchy-icon-container {
        position: absolute;
        top: 0;
        bottom: 0;
        right: 0;
        width: 30px;
        text-align: center;
        display: none
    }
    
    .drop-down-navigation-desktop-panel .page-title .instance-content {
        max-width: 100%;
        display: inline-block
    }
    
    .drop-down-navigation-desktop-panel a {
        color: inherit;
        display: block;
        height: 100%
    }
    
    .drop-down-navigation-desktop-panel-2 {
        text-align: left
    }
    
    .drop-down-navigation-desktop-panel-2 .pages-list {
        position: relative
    }
    
    .drop-down-navigation-desktop-panel-2 .side-bar {
        position: absolute;
        top: 0;
        bottom: 0;
        left: 0;
        width: 13px
    }
    
    .drop-down-navigation-desktop-panel-2 .page-title {
        position: relative;
        margin-left: 28px;
        margin-right: 35px
    }
    
    .drop-down-navigation-desktop-panel-2 .page-item {
        position: relative
    }
    
    .drop-down-navigation-desktop-panel-2 .page-item.state-selected:before {
        content: "";
        top: 0;
        bottom: 0;
        left: 0;
        background: #fff;
        opacity: .1;
        width: 13px;
        position: absolute;
        display: block
    }
    
    .drop-down-navigation-desktop-panel-2 .page-content {
        cursor: pointer
    }
    
    .drop-down-navigation-desktop-panel-2 .page-content:hover .hover-overlay {
        display: block
    }
    
    .drop-down-navigation-desktop-panel-2 .page-item.has-hierarchy>.item-block .sub-hierarchy-icon-container {
        display: inline-block
    }
    
    .drop-down-navigation-desktop-panel-2 .sub-hierarchy-icon-container {
        position: absolute;
        top: 0;
        bottom: 0;
        right: 0;
        width: 30px;
        text-align: center;
        display: none
    }
    
    .drop-down-navigation-desktop-panel-2.color-negative .hover-overlay,.drop-down-navigation-desktop-panel-2.color-negative .page-item.state-selected:before {
        background: #000
    }
    
    .drop-down-navigation-desktop-panel-2 .hover-overlay {
        background: #fff;
        opacity: .1;
        display: none
    }
    
    .drop-down-navigation-desktop-panel-2 a {
        color: inherit;
        display: block;
        height: 100%
    }
    
    .drop-down-navigation-desktop-panel-4 {
        text-align: left
    }
    
    .drop-down-navigation-desktop-panel-4 .pages-list {
        position: relative
    }
    
    .drop-down-navigation-desktop-panel-4 .page-title {
        position: relative;
        margin-left: 20px;
        margin-right: 35px
    }
    
    .drop-down-navigation-desktop-panel-4 .title-container {
        position: relative
    }
    
    .drop-down-navigation-desktop-panel-4 .item-side {
        position: absolute;
        top: 1px;
        right: 0;
        bottom: 0
    }
    
    .drop-down-navigation-desktop-panel-4 .page-item {
        position: relative
    }
    
    .drop-down-navigation-desktop-panel-4 .page-item>.item-block {
        cursor: pointer;
        border-top-style: solid;
        border-top-width: 1px
    }
    
    .drop-down-navigation-desktop-panel-4 .page-item>.item-block:hover .hover-overlay {
        display: block
    }
    
    .drop-down-navigation-desktop-panel-4 .page-item:first-child>.item-block {
        border-top: none
    }
    
    .drop-down-navigation-desktop-panel-4 .page-item:first-child>.item-block .item-side {
        top: 0
    }
    
    .drop-down-navigation-desktop-panel-4 .page-item.has-hierarchy>.item-block .sub-hierarchy-icon-container {
        display: inline-block;
        position: absolute;
        top: 0;
        bottom: 0;
        right: 0;
        width: 30px;
        text-align: center
    }
    
    .drop-down-navigation-desktop-panel-4 .sub-hierarchy-icon-container {
        display: none
    }
    
    .drop-down-navigation-desktop-panel-4.color-negative .hover-overlay,.drop-down-navigation-desktop-panel-4.color-negative .page-item.state-selected:before {
        background: #000
    }
    
    .drop-down-navigation-desktop-panel-4 .page-item.state-selected>.item-block .hover-overlay {
        display: block
    }
    
    .drop-down-navigation-desktop-panel-4 .hover-overlay {
        background: #fff;
        opacity: .1;
        display: none;
        z-index: 1
    }
    
    .drop-down-navigation-desktop-panel-4 a {
        color: inherit;
        display: block;
        height: 100%
    }
    
    .drop-down-navigation-desktop-panel-4 .decorator {
        position: absolute;
        width: 0;
        height: 0;
        border-style: solid;
        border-color: transparent
    }
    
    .horizontal-orientation.drop-down-navigation>.drop-down-navigation-desktop-panel-4>.content-container {
        padding-top: 8px
    }
    
    .side-bottom.drop-down-navigation>.drop-down-navigation-desktop-panel-4>.content-container>.decorator {
        border-width: 0 8px 8px;
        border-color: transparent transparent #007bff;
        top: 0
    }
    
    .side-top.drop-down-navigation>.drop-down-navigation-desktop-panel-4>.content-container {
        padding-top: 0;
        padding-bottom: 8px
    }
    
    .side-top.drop-down-navigation>.drop-down-navigation-desktop-panel-4>.content-container>.decorator {
        border-width: 8px 8px 0;
        border-color: #007bff transparent transparent;
        bottom: 0
    }
    
    .horizontal-center.side-bottom.drop-down-navigation>.drop-down-navigation-desktop-panel-4>.content-container>.decorator,.horizontal-center.side-top.drop-down-navigation>.drop-down-navigation-desktop-panel-4>.content-container>.decorator {
        left: 50%;
        margin-left: -8px
    }
    
    .horizontal-left.side-bottom.drop-down-navigation>.drop-down-navigation-desktop-panel-4>.content-container>.decorator,.horizontal-left.side-top.drop-down-navigation>.drop-down-navigation-desktop-panel-4>.content-container>.decorator {
        left: 8px
    }
    
    .horizontal-right.side-bottom.drop-down-navigation>.drop-down-navigation-desktop-panel-4>.content-container>.decorator,.horizontal-right.side-top.drop-down-navigation>.drop-down-navigation-desktop-panel-4>.content-container>.decorator {
        right: 8px
    }
    
    .vertical-orientation.drop-down-navigation>.drop-down-navigation-desktop-panel-4>.content-container {
        padding-left: 8px
    }
    
    .vertical-orientation.drop-down-navigation>.drop-down-navigation-desktop-panel-4>.content-container>.decorator {
        top: 8px
    }
    
    .side-right.drop-down-navigation>.drop-down-navigation-desktop-panel-4>.content-container>.decorator {
        border-width: 8px 8px 8px 0;
        border-color: transparent #007bff transparent transparent;
        left: 0
    }
    
    .side-left.drop-down-navigation>.drop-down-navigation-desktop-panel-4>.content-container {
        padding-left: 0;
        padding-right: 8px
    }
    
    .side-left.drop-down-navigation>.drop-down-navigation-desktop-panel-4>.content-container>.decorator {
        border-width: 8px 0 8px 8px;
        border-color: transparent transparent transparent #007bff;
        right: 0
    }
    
    .slide-navigation-panel-3 {
        height: 100%;
        position: relative;
        text-align: left
    }
    
    .slide-navigation-panel-3 .close-icon-content {
        position: absolute;
        top: 15px;
        font-size: 14px;
        cursor: pointer
    }
    
    .slide-navigation-panel-3 .side-bar {
        position: absolute;
        top: 0;
        bottom: 0;
        right: 0
    }
    
    .slide-navigation-panel-3 .page-item {
        position: relative
    }
    
    .slide-navigation-panel-3 .page-item:hover .hover-overlay {
        display: block
    }
    
    .slide-navigation-panel-3 .item-side {
        position: absolute;
        top: 0;
        right: 0
    }
    
    .slide-navigation-panel-3 .hierarchy-has-children>.hierarchy-item-content>.hierarchy-item-container .icon-container {
        position: absolute;
        top: 0;
        bottom: 0;
        right: 0;
        display: inline-block;
        width: 40px;
        text-align: center;
        cursor: pointer
    }
    
    .slide-navigation-panel-3 .hierarchy-has-children>.hierarchy-item-content>.hierarchy-item-container .hierarchy-icon {
        width: 40px
    }
    
    .slide-navigation-panel-3 .hierarchy-has-children>.hierarchy-item-content>.hierarchy-item-container .open-icon {
        display: inline-block
    }
    
    .slide-navigation-panel-3 .hierarchy-has-children.open>.hierarchy-item-content>.hierarchy-item-container .open-icon,.slide-navigation-panel-3 .hierarchy-has-children>.hierarchy-item-content>.hierarchy-item-container .close-icon {
        display: none
    }
    
    .slide-navigation-panel-3 .hierarchy-has-children.open>.hierarchy-item-content .hover-overlay,.slide-navigation-panel-3 .hierarchy-has-children.open>.hierarchy-item-content .item-side {
        bottom: 0
    }
    
    .slide-navigation-panel-3 .hierarchy-has-children.open>.hierarchy-item-content>.hierarchy-item-container .close-icon {
        display: inline-block
    }
    
    .slide-navigation-panel-3 .hierarchy-has-children.open>.hierarchy-item-content>.hierarchy-children-container {
        display: block
    }
    
    .slide-navigation-panel-3 .hierarchy-has-children>.hierarchy-item-content>.hierarchy-children-container,.slide-navigation-panel-3 .icon-container {
        display: none
    }
    
    .slide-navigation-panel-3 .page-title {
        padding-left: 25px;
        padding-right: 45px;
        cursor: pointer
    }
    
    .slide-navigation-panel-3 .hierarchy-level-0>.hierarchy-item-content>.hierarchy-item-container .title-container {
        border-bottom-style: solid
    }
    
    .slide-navigation-panel-3 .title-container {
        position: relative;
        z-index: 1
    }
    
    .slide-navigation-panel-3 .header {
        height: 60px;
        position: relative
    }
    
    .slide-navigation-panel-3 .scrolling-pane,.slide-navigation-panel-3 .scrolling-view {
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0
    }
    
    .slide-navigation-panel-3 .scrolling-view {
        top: 60px;
        bottom: 20px
    }
    
    .slide-navigation-panel-3.color-negative .hover-overlay {
        background: #000
    }
    
    .slide-navigation-panel-3 .hover-overlay {
        background: #fff;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=10)";
        filter: alpha(opacity=10);
        -moz-opacity: .1;
        -khtml-opacity: .1;
        opacity: .1;
        zoom:1;display: none;
        z-index: 1
    }
    
    .slide-navigation-panel-3 .page-item.state-selected .hover-overlay {
        display: block
    }
    
    .slide-navigation-panel-3 a {
        color: inherit
    }
    
    .slide-navigation-panel-3.in-animation>.panel-content .slide-scrollbar {
        visibility: hidden
    }
    
    .slide-navigation-panel-3 .slide-scrollbar {
        right: -12px
    }
    
    .percentage-2 .text {
        padding-left: 10px
    }
    
    .percentage-2 .percentage-line,.percentage-2 .percentage-value {
        border-radius: 3px;
        -moz-border-radius: 3px;
        -webkit-border-radius: 3px
    }
    
    .percentage-3 .text {
        display: inline-block;
        padding: 10px;
        vertical-align: middle
    }
    
    .percentage-3 .percentage-line {
        text-align: right;
        width: 100%
    }
    
    .percentage-4 .percentage-item {
        height: 100%;
        display: inline-block;
        text-align: left;
        vertical-align: middle
    }
    
    .percentage-5 .percentage-item {
        display: inline-block;
        text-align: left;
        border-radius: 50%;
        -moz-border-radius: 50%;
        -webkit-border-radius: 50%
    }
    
    .thumb .image-thumb {
        display: inline-block;
        height: 100%;
        cursor: pointer
    }
    
    .thumb .image-thumb .image {
        position: relative;
        display: inline-block;
        width: 100%;
        height: 100%;
        overflow: hidden
    }
    
    .thumb .image-thumb .image img {
        position: relative;
        display: block;
        height: 100%
    }
    
    .thumb .image-thumb .image .current-cover {
        display: none;
        position: absolute
    }
    
    .thumb.current .image-thumb .image .current-cover {
        display: block
    }
    
    .item .image {
        height: 100%
    }
    
    .item .image img {
        display: block;
        height: 100%
    }
    
    .design-element {
        position: absolute
    }
    
    .design-element.footer-element,.design-element.header-element,.design-element.html-section-element,.design-element.page-element,.design-element.page-section-element,.design-element.relative-element {
        position: relative
    }
    
    .design-element.inline-block-element {
        vertical-align: top;
        display: inline-block
    }
    
    .design-element.block-element {
        display: block
    }
    
    .design-element.footer-element,.design-element.header-element,.design-element.html-section-element,.design-element.page-section-element {
        left: 0;
        right: 0
    }
    
    .design-element.tab-element {
        left: 0;
        right: 0;
        top: 0;
        bottom: 0
    }
    
    .design-element.tab-element .element-size-box.tab-element {
        width: 100%;
        height: 100%
    }
    
    .design-element.design-element-inline-block {
        display: inline-block
    }
    
    .background-layers-container-wrapper {
        border-style: solid;
        border-width: 0
    }
    
    .element-background-image,.element-background-layer,.element-background-target-explorer,.element-overlay-layer {
        position: absolute;
        left: 0;
        top: 0;
        right: 0;
        bottom: 0;
        display: block;
        ms-box-sizing: border-box;
        box-sizing: border-box;
        -moz-box-sizing: border-box;
        -webkit-box-sizing: border-box;
        filter: inherit
    }
    
    .element-background-layer-hidden {
        display: none
    }
    
    .content-container,.design-element-main-box,.element-border-box,.html-element {
        position: relative;
        margin: 0;
        height: 100%;
        ms-box-sizing: border-box;
        box-sizing: border-box;
        -moz-box-sizing: border-box;
        -webkit-box-sizing: border-box;
        filter: inherit
    }
    
    .html-element {
        display: block!important
    }
    
    .page-element-border-box {
        position: relative;
        filter: inherit
    }
    
    .element-border-target {
        border-width: 0
    }
    
    .element-background-image,.element-background-layer,.element-overlay-layer {
        background-origin: padding-box;
        background-clip: padding-box;
        border-style: solid;
        border-color: transparent;
        border-width: 0
    }
    
    .element-background-image {
        overflow: hidden
    }
    
    .design-element-content-box {
        height: 100%;
        margin: 0;
        position: relative
    }
    
    .element-content-box {
        white-space: nowrap
    }
    
    body .page-content-container,body .page-element {
        position: relative;
        height: auto
    }
    
    body .design-element.page-content-element {
        position: relative
    }
    
    body .design-element.is-in-cell-item {
        position: relative;
        top: 0!important
    }
    
    .absolute-arrangement .instance-container,.content-marking {
        position: absolute
    }
    
    body .design-element .element-size-box.is-cell-item-size-box.is-size-box-inline-block,body .design-element.is-in-cell-item.design-element-inline-block {
        max-width: 100%
    }
    
    body.mobile-desktop-mode .page-content-element-size-box {
        width: 100%!important
    }
    
    .hidden-design-element {
        display: none!important
    }
    
    .content-marking {
        left: -1px;
        top: -1px;
        bottom: -1px;
        right: -1px
    }
    
    body.express-mode .content-marking,body.preview-mode .content-marking {
        display: none
    }
    
    .content-marking-front {
        border: 1px dashed #000
    }
    
    .content-marking-back {
        border: 1px solid #fff
    }
    
    .relative-arrangement .instance-container {
        position: relative;
        vertical-align: top;
        display: inline-block
    }
    
    .design-element-rotation-wrapper {
        margin: 0;
        height: 100%;
        display: block
    }
    
    .margin-marking.not-active,body.state-attaching-to-different-container .margin-marking {
        display: none
    }
    
    .has-text-transform-uppercase {
        text-transform: uppercase
    }
    
    .has-text-transform-capitalize {
        text-transform: capitalize
    }
    
    .has-text-is-bold {
        font-weight: 700
    }
    
    .has-text-is-italic {
        font-style: italic
    }
    
    .has-text-is-underline {
        text-decoration: underline
    }
    
    .has-text-is-line-through {
        text-decoration: line-through
    }
    
    .design-element .failed-to-load-message .inner-text .is-action:hover,.has-text-is-underline .rich-text-content,.label-text-underline,.store-breadcrumb-element .bread-crumb-element:hover .underline,.store-categories-element>.element-container .category-element:hover,.store-filters-element:hover,a.design-element-link-part.has-underline-children:hover .rich-text-content {
        text-decoration: underline
    }
    
    .margin-marking {
        position: absolute;
        z-index: 99988
    }
    
    .margin-marking .margin-marking-line {
        background: url(images/animated-dash-red-white.gif)!important;
        position: absolute
    }
    
    .margin-marking.left,.margin-marking.right {
        top: 0;
        bottom: 0
    }
    
    .margin-marking.left .margin-marking-line,.margin-marking.right .margin-marking-line {
        left: 0;
        right: 0;
        top: 50%;
        margin-top: -1px;
        height: 2px
    }
    
    .margin-marking.bottom,.margin-marking.top {
        left: 0;
        right: 0
    }
    
    .margin-marking.bottom .margin-marking-line,.margin-marking.top .margin-marking-line {
        top: 0;
        bottom: 0;
        left: 50%;
        margin-left: -1px;
        width: 2px
    }
    
    .margin-marking.left.negative {
        left: 0
    }
    
    .margin-marking.left.positive {
        right: 100%
    }
    
    .margin-marking.left.center-margin.negative {
        left: 50%
    }
    
    .margin-marking.left.center-margin.positive {
        right: 50%
    }
    
    .margin-marking.top.negative {
        top: 0
    }
    
    .margin-marking.top.positive {
        bottom: 100%
    }
    
    .margin-marking.top.center-margin.negative {
        top: 50%
    }
    
    .margin-marking.top.center-margin.positive {
        bottom: 50%
    }
    
    .margin-marking.right.negative {
        right: 0
    }
    
    .margin-marking.right.positive {
        left: 100%
    }
    
    .margin-marking.bottom.negative {
        bottom: 0
    }
    
    .margin-marking.bottom.positive {
        top: 100%
    }
    
    body.view-mode .webzai-clickable-behaviour {
        cursor: pointer;
        -moz-user-select: none
    }
    
    body.view-mode .webzai-clickable-behaviour * {
        cursor: inherit
    }
    
    a.design-element-link-part {
        display: block;
        position: relative;
        margin: 0;
        height: 100%
    }
    
    .design-element.element-empty-state {
        visibility: hidden
    }
    
    .design-element .failed-to-load-message {
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        height: 240px;
        text-align: center;
        font-size: 16px;
        line-height: 40px;
        color: #747474;
        text-transform: uppercase;
        font-weight: 700;
        white-space: nowrap;
        overflow: hidden;
        text-overflow: ellipsis;
        z-index: 100;
        border: 2px solid #656565;
        background-color: #f9f9f9
    }
    
    .design-element .failed-to-load-message .inner-text {
        top: 50%;
        margin-top: -20px;
        left: 0;
        position: absolute;
        right: 0
    }
    
    .design-element .failed-to-load-message .inner-text .is-action {
        cursor: pointer;
        color: #00f
    }
    
    .fit-to-size.data-list-item.design-element,.fit-to-size.skin-hierarchy-box.design-element {
        left: 0;
        top: 0
    }
    
    .view-mode .data-list-item.design-element .skin-hierarchy-box.design-element {
        position: relative!important;
        margin: 0!important;
        height: 100%!important
    }
    
    .view-mode .data-list-item.design-element .skin-hierarchy-box.design-element .template-item.element-size-box {
        width: auto!important;
        min-height: 0!important
    }
    
    .iframe-content-block {
        display: block;
        border: none;
        position: absolute;
        left: 0;
        top: 0;
        width: 100%;
        height: 100%;
        margin: 0;
        padding: 0
    }
    
    .iframe-content-wrapper {
        overflow: auto
    }
    
    .iframe-content-wrapper.scrolling-yes {
        -webkit-overflow-scrolling: touch
    }
    
    .design-element.skin-element .skin-instance-controller {
        position: absolute;
        width: 100%;
        height: 100%;
        top: 0;
        left: 0
    }
    
    .menu-sub-hierarchy {
        z-index: 100
    }
    
    .menu-sub-hierarchy .menu-sub-hierarchy-arrow {
        margin: 0 7px
    }
    
    body.view-mode .menu-button-cursor-pointer {
        cursor: pointer
    }
    
    .label-element.state-editing,.preview-mode .rich-text-content,.rich-text-content.editing-mode {
        cursor: text
    }
    
    .base-page-content-element .main-sections-container {
        display: inline-block;
        width: 100%
    }
    
    .side-bar-page-content-element.right-side-bar .side-bar-background-layer {
        right: 0
    }
    
    .side-bar-page-content-element .side-bar-background-layer {
        position: absolute;
        height: 100%
    }
    
    .side-bar-page-content-element .main-sections-container,.side-bar-page-content-element .side-bar-sections-container {
        overflow: hidden
    }
    
    .label-text-bold {
        font-weight: 700
    }
    
    .label-text-italic {
        font-style: italic
    }
    
    .label-element .text-content {
        line-height: normal;
        width: 100%;
        white-space: pre-wrap;
        word-wrap: break-word
    }
    
    .label-element .text-content:after {
        content: "";
        position: absolute;
        left: 0;
        right: 0;
        bottom: 0;
        top: 0
    }
    
    .label-element .element-text-input {
        border: none;
        padding: 0;
        overflow: hidden;
        background-color: transparent;
        white-space: pre-wrap;
        word-wrap: break-word;
        width: 100%
    }
    
    .mobile-desktop-mode .row-element.root-row.last {
        margin-bottom: 0!important
    }
    
    .rich-text-positioning-wrapper {
        position: absolute;
        left: 0;
        right: 0
    }
    
    .rich-text-positioning-wrapper.vertical-alignment-top {
        top: 0
    }
    
    .rich-text-positioning-wrapper.vertical-alignment-bottom {
        bottom: 0
    }
    
    .rich-text-positioning-wrapper.vertical-alignment-center {
        top: 50%
    }
    
    @media only screen and (max-device-width: 480px) {
        .rich-text-element-content {
            -webkit-text-size-adjust:100%
        }
    }
    
    .rich-text-content a.wz-link {
        text-decoration: none;
        color: inherit
    }
    
    .rich-text-content a[data-attached-link] {
        color: inherit!important
    }
    
    .rich-content-element .rich-content {
        position: absolute;
        left: 0;
        right: 0;
        text-align: left
    }
    
    #body-element .rich-content-element .rich-content a *,#body-element .rich-content-element .theme-inline-text-style-marked * {
        color: inherit
    }
    
    .design-element.page-element {
        display: block;
        text-align: left;
        position: relative;
        z-index: 1
    }
    
    .fixed-page-background {
        border: none!important
    }
    
    body {
        background-color: #fff
    }
    
    body.design-mode .design-element {
        z-index: inherit!important
    }
    
    body.view-mode .design-element.page-element {
        overflow: hidden
    }
    
    body.full-screen-view .fixed-page-background,body.view-mode .fixed-page-background {
        left: 0;
        top: 0
    }
    
    body.full-screen-view.pc-desktop-mode .fixed-page-background,body.full-screen-view.site-viewer .fixed-page-background,body.view-mode.pc-desktop-mode .fixed-page-background,body.view-mode.site-viewer .fixed-page-background {
        position: fixed
    }
    
    body.inner-screen-view .fixed-page-background.fixed-attachment-background .image-box-image-wrapper {
        position: absolute;
        width: 100%!important;
        height: 100%!important;
        left: 0;
        top: 0;
        background-attachment: fixed
    }
    
    body.inner-screen-view .fixed-page-background.sticky-background {
        left: 50%
    }
    
    body.inner-screen-view .fixed-page-background.sticky-background.fixed-to-top {
        position: absolute;
        top: 0
    }
    
    body.inner-screen-view .fixed-page-background.sticky-background.fixed-to-bottom {
        position: absolute;
        bottom: 0;
        top: auto
    }
    
    body.inner-screen-view .fixed-page-background.sticky-background.fixed-to-center {
        position: fixed;
        top: 0;
        bottom: auto
    }
    
    .view-mode .design-element.positioned-fixed {
        position: fixed!important
    }
    
    .view-mode .design-element.positioned-fixed.footer-element {
        bottom: 0
    }
    
    .view-mode .design-element.animation-fixed {
        position: absolute!important
    }
    
    .page-resize-grip-bottom .resize-grip-line {
        top: 4px
    }
    
    .page-content-decorator {
        left: 50%;
        position: absolute
    }
    
    #google_translate_element {
        position: fixed;
        z-index: 10000001
    }
    
    .icon-element-content {
        text-align: center;
        position: absolute;
        top: 50%;
        left: 0;
        right: 0
    }
    
    .line-element-line {
        position: absolute
    }
    
    .line-element-line.vertical {
        top: 0;
        bottom: 0;
        width: 0;
        left: 50%
    }
    
    .line-element-line.horizontal {
        left: 0;
        right: 0;
        height: 0;
        top: 50%
    }
    
    .canvas-ellipse {
        -moz-box-shadow: none!important;
        -webkit-box-shadow: none!important;
        box-shadow: none!important
    }
    
    .border-radius-ellipse,body.html4 .border-radius-ellipse {
        -moz-border-radius: 50%!important;
        -webkit-border-radius: 30px!important;
        border-radius: 50%!important;
        border-style: solid
    }
    
    .preview-mode .popupOpener .design-element {
        cursor: pointer
    }
    
    body.state-hierarchy-editing .design-element.template-box {
        top: 0;
        left: 0;
        position: relative
    }
    
    body.view-mode .design-element.video-player .video-icon-holder {
        cursor: pointer
    }
    
    body.view-mode .design-element.video-player .video-icon-holder:hover .icon {
        display: inline-block;
        background: url(viewer-sprite.png) top left no-repeat;
        background-position: 0 0!important;
        width: 42px;
        height: 29px
    }
    
    .switch-panel-element .ui-effects-wrapper {
        z-index: auto
    }
    
    .app-iframe {
        border: none;
        position: absolute;
        left: 0;
        top: 0;
        width: 100%;
        height: 100%;
        margin: 0;
        padding: 0;
        overflow: hidden;
        display: block
    }
    
    .app-iframe.auto-scrollbars {
        overflow: auto
    }
    
    .captcha-element {
        margin-top: 10px;
        height: 80px!important
    }
    
    .captcha-element>div {
        margin: 0 auto;
        padding: 3px
    }
    
    .design-mode .captcha-element {
        pointer-events: none
    }
    
    .captcha-error>div {
        border: 2px solid red;
        border-radius: 2px;
        padding: 2px 0 0 2px
    }
    
    .mobile-desktop-mode .captcha-element>div {
        -moz-transform: scale(.77);
        -webkit-transform: scale(.77);
        -ms-transform: scale(.77);
        transform: scale(.77);
        transform-origin: left
    }
    
    .design-element .design-element.skin-hierarchy-box {
        position: absolute;
        width: 100%;
        height: 100%;
        top: 0;
        left: 0
    }
    
    .paypal-button {
        width: 100%;
        height: 100%;
        border-color: transparent!important;
        padding: 0!important;
        background-color: transparent!important
    }
    
    .out-of-stock-overlay {
        visibility: hidden
    }
    
    .out-of-stock .out-of-stock-overlay {
        position: absolute;
        visibility: visible;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background-color: rgba(255,255,255,.75);
        z-index: 20
    }
    
    .out-of-stock .out-of-stock-message {
        top: 50%;
        position: absolute;
        line-height: 2;
        font-size: 16px;
        font-weight: 700;
        color: #000;
        text-align: center;
        left: 0;
        right: 0;
        margin-top: -20px
    }
    
    .store-front-element .failed-to-load-message {
        text-transform: none
    }
    
    .store-front-element .failed-to-load-message .description {
        font-size: 16px;
        line-height: 1.36;
        white-space: normal
    }
    
    .hideable-text-detail .common-rich-content-style {
        white-space: initial
    }
    
    .hideable-text-detail .common-rich-content-style p {
        display: block;
        -webkit-margin-before: 1em;
        -webkit-margin-after: 1em;
        -webkit-margin-start: 0;
        -webkit-margin-end: 0
    }
    
    .store-price-element .default-font {
        font-family: Tahoma,Geneva,sans-serif!important
    }
    
    .store-breadcrumb-element {
        z-index: 98!important;
        min-width: 100px;
        white-space: normal
    }
    
    .store-categories-container,.store-filters-element.no-background {
        z-index: 99!important
    }
    
    .store-breadcrumb-element.with-children {
        margin-top: 16px;
        margin-bottom: 8px
    }
    
    .store-breadcrumb-element .bread-crumb-element {
        display: inline-block
    }
    
    .store-breadcrumb-element .bread-crumb-element.with-child {
        position: relative
    }
    
    .store-breadcrumb-element .bread-crumb-element.with-child:after {
        content: '>';
        margin-left: 5px;
        margin-right: 5px
    }
    
    .store-categories-container.with-overlay:after {
        content: 'This is where your categories & filters are shown when enabled in the Store.';
        font-size: 15px;
        color: #000;
        white-space: normal;
        position: absolute;
        text-align: center;
        display: block;
        margin-top: -10px;
        top: 50%;
        left: 0;
        right: 0;
        z-index: 100
    }
    
    .store-categories-container.with-overlay:before {
        position: absolute;
        top: 0;
        content: '';
        left: 0;
        right: 0;
        bottom: 0;
        border-style: dashed;
        border-width: 1px;
        border-color: #aaa;
        background-color: rgba(255,255,255,.9);
        z-index: 100
    }
    
    .mobile-desktop-mode .store-categories-container .row-element.desc-row {
        margin-bottom: 0
    }
    
    .mobile-desktop-mode .store-categories-container .row-element .cell-element-container {
        padding: 0
    }
    
    body.design-mode .store-categories-container {
        z-index: 1!important
    }
    
    .store-categories-element {
        z-index: 101!important;
        text-align: center;
        width: 100%
    }
    
    .store-categories-element>.element-container {
        display: inline-block
    }
    
    .store-categories-element>.element-container .category-element {
        min-height: 33px;
        line-height: 33px;
        cursor: pointer;
        padding: 0 12px;
        display: inline-block;
        position: relative;
        float: left;
        font-weight: 400;
        border: 1px solid transparent;
        font-size: 14px
    }
    
    .store-categories-element>.element-container .category-element span.active {
        font-weight: 700
    }
    
    .store-categories-element>.element-container .category-element .subcategories {
        display: none;
        position: absolute;
        top: 34px;
        left: -1px;
        background-color: #fff;
        padding: 12px;
        border: 1px solid #ccc;
        color: #333
    }
    
    .store-categories-element>.element-container .category-element .subcategories .categories-backdrop {
        position: fixed;
        left: 0;
        right: 0;
        top: 0;
        bottom: 0;
        z-index: -1
    }
    
    .store-categories-element>.element-container .category-element .subcategories .category-element {
        min-height: 20px;
        line-height: 20px;
        padding: 8px;
        display: block;
        float: none;
        text-align: left
    }
    
    .store-categories-element>.element-container .category-element .subcategories .category-element.submenu-with-children {
        opacity: .7;
        font-weight: 700;
        padding: 8px 8px 4px;
        float: none;
        display: block;
        text-align: left
    }
    
    .store-categories-element>.element-container .category-element .subcategories .category-element.submenu-with-children.active {
        opacity: 1
    }
    
    .store-categories-element>.element-container .category-element .subcategories .category-element .element-container .element-container .category-element {
        min-height: 20px;
        line-height: 20px
    }
    
    .store-categories-element>.element-container .category-element .subcategories .element-container {
        min-height: 20px;
        line-height: 20px;
        display: block;
        text-align: left
    }
    
    .store-categories-element>.element-container .category-element .subcategories .submenu-inner-child {
        padding: 0 8px
    }
    
    .store-categories-element>.element-container .category-element.hover {
        color: #333;
        z-index: 1
    }
    
    .store-categories-element>.element-container .category-element.hover .subcategories {
        display: block
    }
    
    .store-categories-element>.element-container .category-element.active {
        font-weight: 700;
        opacity: 1
    }
    
    .store-categories-element>.element-container>.category-element.with-children.hover {
        border: 1px solid #ccc;
        background-color: #fff
    }
    
    .store-categories-element>.element-container>.category-element.with-children.hover:after {
        content: '';
        position: absolute;
        bottom: -2px;
        height: 3px;
        left: 0;
        right: 0;
        background-color: #fff
    }
    
    .design-mode .store-categories-element {
        overflow: hidden
    }
    
    .design-mode .store-categories-element .category-element {
        float: none
    }
    
    .store-filters-element {
        z-index: 100!important
    }
    
    .store-filters-element .filter-click-background {
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        z-index: -1;
        display: none
    }
    
    .store-filters-element .dropdown-wrapper {
        min-width: 130px;
        position: relative;
        display: inline-block;
        border-radius: 3px;
        margin-right: 8px;
        margin-top: 8px;
        margin-bottom: 8px;
        float: left
    }
    
    .store-filters-element .dropdown-wrapper .popover {
        display: none;
        position: absolute;
        top: 30px;
        min-width: 130px
    }
    
    .store-filters-element .dropdown-wrapper .real-dropdown div {
        height: 33px;
        min-width: 130px;
        color: #333;
        -webkit-appearance: none;
        border: 1px solid #ccc;
        display: inline-block;
        float: left;
        background-color: #fafafa;
        line-height: 33px;
        box-sizing: border-box;
        padding-left: 10px;
        border-radius: 3px;
        padding-right: 20px
    }
    
    .store-filters-element .dropdown-wrapper .real-dropdown div .filter-label {
        font-weight: 700
    }
    
    .store-filters-element .dropdown-wrapper.active {
        z-index: 1
    }
    
    .store-filters-element .dropdown-wrapper.active .filter-click-background,.store-filters-element .dropdown-wrapper.active .popover {
        display: block
    }
    
    .store-filters-element .dropdown-wrapper .fake-dropdown {
        -webkit-box-sizing: border-box;
        background: #fff;
        box-sizing: border-box;
        display: block;
        overflow: hidden;
        padding-right: 30px;
        position: absolute;
        left: 0;
        right: 0;
        top: 0;
        bottom: 0;
        pointer-events: none
    }
    
    .store-filters-element .dropdown-wrapper .fake-dropdown .fake-select {
        height: 33px;
        line-height: 33px;
        overflow: hidden;
        font-size: 14px;
        padding: 0 5px 0 12px;
        white-space: nowrap;
        text-overflow: ellipsis
    }
    
    .store-filters-element .dropdown-wrapper .fake-dropdown .fake-select:after {
        border-color: #707070 transparent transparent;
        border-style: solid;
        border-width: 5px;
        content: "";
        margin-top: -3px;
        position: absolute;
        right: 10px;
        top: 50%
    }
    
    .store-filters-element .dropdown-wrapper:hover {
        cursor: pointer
    }
    
    .store-filters-element .dropdown-wrapper:after {
        position: absolute;
        right: 7px;
        top: 14px;
        content: '';
        pointer-events: none;
        width: 0;
        height: 0;
        border-left: 5px solid transparent;
        border-right: 5px solid transparent;
        border-top: 7px solid #777
    }
    
    .store-filters-element.active {
        font-weight: 700
    }
    
    .store-filters-element.no-background .dropdown-wrapper:after {
        top: 7px
    }
    
    .store-filters-element.no-background .real-dropdown>div {
        background-color: transparent;
        border: none;
        color: inherit;
        height: 20px;
        line-height: 20px;
        padding-left: 0
    }
    
    .store-filters-element.open {
        z-index: 102!important
    }
    
    .mobile-desktop-mode .store-filters-element {
        z-index: 101!important
    }
    
    .mobile-desktop-mode .store-filters-element .real-dropdown>div {
        height: auto
    }
    
    .mobile-desktop-mode .store-filters-element .dropdown-wrapper {
        text-align: left;
        min-width: 30px;
        width: 100%
    }
    
    .mobile-desktop-mode .store-filters-element .dropdown-wrapper .real-dropdown div {
        min-width: 50px
    }
    
    .mobile-desktop-mode .store-filters-element .dropdown-wrapper .real-dropdown div .filter-label {
        display: block;
        line-height: 1.4;
        font-size: 11px;
        font-weight: 400
    }
    
    .mobile-desktop-mode .store-filters-element .dropdown-wrapper .real-dropdown div .filter-text {
        font-weight: 700;
        position: relative
    }
    
    .mobile-desktop-mode .store-filters-element .dropdown-wrapper:after {
        display: none
    }
    
    .mobile-desktop-mode .store-filters-element.open {
        z-index: 102!important
    }
    
    .mobile-desktop-mode .filter-button span {
        font-weight: 700;
        position: relative;
        text-transform: uppercase
    }
    
    .design-mode .store-filters-element {
        overflow: hidden
    }
    
    .design-mode .store-filters-element .dropdown-wrapper {
        float: none
    }
    
    .store-footer-buttons span {
        float: right;
        font-size: 15px;
        padding: 12px 24px;
        margin-top: 10px
    }
    
    .store-footer-buttons span:first-child {
        clear: both
    }
    
    .store-selected-filters-element .filter-label {
        border-radius: 15px;
        background-color: #eee;
        padding: 5px 10px;
        font-size: 14px;
        margin-right: 10px;
        -moz-user-select: none;
        user-select: none;
        border: 1px solid transparent
    }
    
    .store-selected-filters-element .filter-label:after {
        content: '\00D7';
        border-radius: 50%;
        background-color: #a5a5a5;
        margin-left: 8px;
        width: 20px;
        line-height: 20px;
        display: inline-block;
        text-align: center;
        color: #fff
    }
    
    .popover li a,.store-selected-filters-element .clear-all {
        line-height: 30px
    }
    
    .store-selected-filters-element .filter-label:hover {
        background-color: #ddd
    }
    
    .store-selected-filters-element .clear-all,.store-selected-filters-element .filter-label {
        margin-top: 8px;
        float: left
    }
    
    .mobile-desktop-mode .store-selected-filters-element .filter-label {
        padding: 0 8px
    }
    
    .mobile-desktop-mode .store-selected-filters-element .filter-label:after {
        line-height: 12px;
        width: 12px
    }
    
    .mobile-desktop-mode .store-selected-filters-element .clear-all {
        line-height: 16px
    }
    
    .popover {
        background-color: #fff;
        color: #333;
        padding: 15px;
        border: 1px solid #ccc;
        box-sizing: border-box;
        max-width: 300px
    }
    
    .popover li label:hover,.popover li.filter-label:hover {
        background-color: rgba(0,0,0,.05)
    }
    
    .popover li {
        list-style-type: none
    }
    
    .popover li.filter-label {
        height: 32px;
        line-height: 32px
    }
    
    .popover li input {
        visibility: hidden;
        width: 0;
        height: 0
    }
    
    .popover li label {
        display: block;
        height: 30px
    }
    
    .popover li label .choice-checkbox {
        height: 14px;
        width: 14px;
        border: 1px solid #777;
        display: inline-block;
        border-radius: 2px;
        cursor: pointer;
        margin-top: 7px;
        position: relative
    }
    
    .popover li label .choice-checkbox:after {
        font-size: 14px;
        line-height: 14px;
        content: '';
        background-image: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path fill="white" d="M20.285 2l-11.285 11.567-5.286-5.011-3.714 3.716 9 8.728 15-15.285z"/></svg>');
        background-size: cover;
        background-position: center;
        width: 14px;
        height: 14px;
        left: 0;
        display: inline-block;
        position: absolute;
        visibility: hidden;
        color: #fff
    }
    
    .popover li label.darkCheckmark .choice-checkbox:after {
        background-image: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path fill="black" d="M20.285 2l-11.285 11.567-5.286-5.011-3.714 3.716 9 8.728 15-15.285z"/></svg>')
    }
    
    .popover li.square {
        display: inline-block;
        float: left;
        margin: 5px;
        cursor: pointer;
        -moz-transform: scale(1) translate3d(0,0,0);
        -webkit-transform: scale(1) translate3d(0,0,0);
        -ms-transform: scale(1) translate3d(0,0,0);
        transform: scale(1) translate3d(0,0,0);
        -webkit-transition: transform .2s ease-out;
        -moz-transition: transform .2s ease-out;
        -ms-transition: transform .2s ease-out;
        -o-transition: transform .2s ease-out;
        transition: transform .2s ease-out
    }
    
    .popover li.square:hover {
        -moz-transform: scale(1.2) translate3d(0,0,0);
        -webkit-transform: scale(1.2) translate3d(0,0,0);
        -ms-transform: scale(1.2) translate3d(0,0,0);
        transform: scale(1.2) translate3d(0,0,0)
    }
    
    .popover li.square label {
        width: 26px;
        height: 26px
    }
    
    .popover li.square label .choice-checkbox {
        margin: 0;
        width: 100%;
        height: 100%
    }
    
    .popover li.square label .choice-checkbox:after {
        margin-left: 6px;
        margin-top: 6px
    }
    
    .popover li a {
        margin-left: 10px;
        text-decoration: none;
        color: inherit;
        vertical-align: top;
        pointer-events: none;
        display: inline-block
    }
    
    .popover li input[type=checkbox]:checked+label>.choice-checkbox:after {
        visibility: visible
    }
    
    .popover .popover-item {
        line-height: 40px;
        position: relative;
        cursor: pointer
    }
    
    .popover .popover-item:hover {
        text-decoration: underline
    }
    
    .popover .popover-item:active {
        background-color: #eee
    }
    
    .popover .popover-item.has-page:after {
        position: absolute;
        right: 7px;
        top: 17px;
        content: '';
        pointer-events: none;
        width: 0;
        height: 0;
        border-top: 5px solid transparent;
        border-bottom: 5px solid transparent;
        border-left: 7px solid #777
    }
    
    .popover .title {
        font-weight: 700;
        font-size: 15px;
        line-height: 2
    }
    
    .popover.right-align {
        right: 0
    }
    
    .popover.small-width {
        width: auto
    }
    
    .mobile-desktop-mode .popover {
        width: 80vw;
        overflow: auto;
        max-height: calc(100vh - 84px)
    }
    
    .mobile-desktop-mode .popover.small-width {
        width: auto
    }
    
    .site-editor.mobile-desktop-mode .popover {
        max-height: 520px
    }
    
    .store-variants-container {
        z-index: 0!important
    }
    
    .store-variants-container .element-filter-container {
        top: 0
    }
    
    .store-variants-container .store-variant-row {
        white-space: initial;
        text-align: left
    }
    
    .store-variants-container .store-variant-row .store-variant-name {
        margin: 15px 0 0;
        font-size: 14px
    }
    
    .store-variants-container .store-variant-row .dropdown-wrapper {
        width: 230px;
        position: relative;
        margin-top: 5px;
        border: 1px solid #ddd
    }
    
    .store-variants-container .store-variant-row .dropdown-wrapper .fake-dropdown {
        -webkit-box-sizing: border-box;
        background: #fff;
        box-sizing: border-box;
        display: block;
        overflow: hidden;
        padding-right: 30px;
        position: absolute;
        left: 0;
        right: 0;
        top: 0;
        bottom: 0;
        pointer-events: none
    }
    
    .store-variants-container .store-variant-row .dropdown-wrapper .fake-dropdown .fake-select {
        border-right: 1px dashed #ddd;
        height: 42px;
        line-height: 42px;
        overflow: hidden;
        font-size: 14px;
        padding: 0 5px 0 12px;
        white-space: nowrap;
        text-overflow: ellipsis
    }
    
    .store-variants-container .store-variant-row .dropdown-wrapper .fake-dropdown .fake-select:after {
        border-color: #707070 transparent transparent;
        border-style: solid;
        border-width: 5px;
        content: "";
        margin-top: -3px;
        position: absolute;
        right: 10px;
        top: 50%
    }
    
    .store-variants-container .store-variant-row .dropdown-wrapper .real-dropdown select {
        height: 42px;
        width: 230px;
        -webkit-appearance: none
    }
    
    .store-variants-container .store-variant-row .dropdown-wrapper:hover {
        border: 1px solid #444;
        cursor: pointer
    }
    
    .store-variants-container .store-variant-row .store-variant-square {
        height: 42px;
        min-width: 42px;
        text-align: center;
        font-size: 15px;
        line-height: 38px;
        margin-top: 10px;
        display: inline-block;
        position: relative;
        margin-right: 13px;
        margin-left: 2px;
        box-sizing: border-box
    }
    
    .store-variants-container .store-variant-row .store-variant-square:first-child {
        margin-left: 4px
    }
    
    .store-variants-container .store-variant-row .store-variant-square.out-of-stock {
        opacity: .3;
        position: relative
    }
    
    .store-variants-container .store-variant-row .store-variant-square.out-of-stock:after {
        position: absolute;
        content: "";
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background-image: url('data:image/svg+xml;utf8,<svg version=\"1.1\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\"><line x1=\"100%\" y1=\"100%\" x2=\"0\" y2=\"0\" style=\"stroke:rgb(255,255,255);stroke-width:4\"/></svg>');
        background-size: cover;
        background-position: center
    }
    
    .store-variants-container .store-variant-row .store-variant-square.out-of-stock.dark:after {
        background-image: url('data:image/svg+xml;utf8,<svg version=\"1.1\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\"><line x1=\"100%\" y1=\"100%\" x2=\"0\" y2=\"0\" style=\"stroke:rgb(0,0,0);stroke-width:4\"/></svg>')
    }
    
    .store-variants-container .store-variant-row .store-variant-square:hover {
        outline: solid 2px;
        cursor: pointer
    }
    
    .multi-color-background {
        background-size: cover;
        background-position: center;
        background-image: url("data:image/svg+xml,%3Csvg%20width='62px'%20height='62px'%20viewBox='0%200%2062%2062'%20version='1.1'%20xmlns='http://www.w3.org/2000/svg'%20xmlns:xlink='http://www.w3.org/1999/xlink'%3E%3Cdefs%3E%3Crect%20id='path-1'%20x='0'%20y='0'%20width='62'%20height='62'%3E%3C/rect%3E%3C/defs%3E%3Cg%20id='Page-1'%20stroke='none'%20stroke-width='1'%20fill='none'%20fill-rule='evenodd'%3E%3Cg%20id='Group'%3E%3Cmask%20id='mask-2'%20fill='white'%3E%3Cuse%20xlink:href='%23path-1'%3E%3C/use%3E%3C/mask%3E%3Cuse%20id='Mask'%20fill='%23D8D8D8'%20xlink:href='%23path-1'%3E%3C/use%3E%3Cg%20mask='url(%23mask-2)'%3E%3Cg%20transform='translate(-34.720000,%20-34.720000)'%3E%3Cpolyline%20id='Path'%20fill='%23F30940'%20points='64.48%2018.9923438%2064.48%2066.6403147%20110.548906%2018.6'%3E%3C/polyline%3E%3Cpolyline%20id='Path'%20fill='%23FDAE00'%20transform='translate(97.565274,%2062.966769)%20rotate(40.000000)%20translate(-97.565274,%20-62.966769)%20'%20points='74.5308212%2039.3389555%2074.5308212%2086.9869265%20120.599727%2038.9466118'%3E%3C/polyline%3E%3Cpolyline%20id='Path-Copy'%20fill='%23F4EE00'%20transform='translate(90.895128,%2085.135565)%20rotate(80.000000)%20translate(-90.895128,%20-85.135565)%20'%20points='67.8606749%2061.507751%2067.8606749%20109.155722%20113.929581%2061.1154072'%3E%3C/polyline%3E%3Cpolyline%20id='Path-Copy-2'%20fill='%23B5D719'%20transform='translate(73.239293,%2098.918500)%20rotate(120.000000)%20translate(-73.239293,%20-98.918500)%20'%20points='50.2048399%2075.2906866%2050.2048399%20122.938658%2096.2737462%2074.8983429'%3E%3C/polyline%3E%3Cpolyline%20id='Path-Copy-3'%20fill='%2363CAC7'%20transform='translate(50.940683,%2098.649812)%20rotate(160.000000)%20translate(-50.940683,%20-98.649812)%20'%20points='27.9062302%2075.021998%2027.9062302%20122.669969%2073.9751364%2074.6296542'%3E%3C/polyline%3E%3Cpolyline%20id='Path-Copy-4'%20fill='%230089C7'%20transform='translate(36.060683,%2080.049812)%20rotate(200.000000)%20translate(-36.060683,%20-80.049812)%20'%20points='13.0262302%2056.421998%2013.0262302%20104.069969%2059.0951364%2056.0296542'%3E%3C/polyline%3E%3Cpolyline%20id='Path-Copy-5'%20fill='%2335419F'%20transform='translate(32.319293,%2057.998500)%20rotate(240.000000)%20translate(-32.319293,%20-57.998500)%20'%20points='9.28483991%2034.3706866%209.28483991%2082.0186576%2055.3537462%2033.9783429'%3E%3C/polyline%3E%3Cpolyline%20id='Path-Copy-6'%20fill='%238149A1'%20transform='translate(46.255128,%2040.495565)%20rotate(280.000000)%20translate(-46.255128,%20-40.495565)%20'%20points='23.2206749%2016.867751%2023.2206749%2064.5157219%2069.2895811%2016.4754072'%3E%3C/polyline%3E%3Cpolyline%20id='Path-Copy-7'%20fill='%23CA3597'%20transform='translate(66.565274,%2033.206769)%20rotate(320.000000)%20translate(-66.565274,%20-33.206769)%20'%20points='43.5308212%209.57895552%2043.5308212%2057.2269265%2089.5997275%209.18661177'%3E%3C/polyline%3E%3C/g%3E%3C/g%3E%3C/g%3E%3C/g%3E%3C/svg%3E")
    }
    
    .breadcrumb-element>.breadcrumb-title:hover {
        text-decoration: underline!important
    }
    
    .facebook-timeline-element .facebook-media-element .type-image {
        background-size: cover;
        background-position: top
    }
    
    .facebook-timeline-element .facebook-media-element .link-icon,.facebook-timeline-element .facebook-media-element .type-image,.facebook-timeline-element .facebook-media-element .type-link,.facebook-timeline-element .facebook-media-element .type-video {
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0
    }
    
    .facebook-timeline-element .facebook-media-element .link-icon .viewer-font-icon {
        width: 70px;
        height: 70px;
        margin: -45px 0 0 -45px;
        font-size: 70px;
        background: rgba(0,0,0,.6);
        color: #fff;
        zoom:1;transition: opacity .1s;
        border-radius: 50%;
        position: absolute;
        left: 50%;
        top: 50%;
        border: 2px solid #fff
    }
    
    .facebook-timeline-element .facebook-media-element .link-icon .viewer-font-icon.viewer-font-icon-link {
        font-size: 40px
    }
    
    .facebook-timeline-element .facebook-media-element .link-icon .viewer-font-icon.viewer-font-icon-link:before {
        margin-left: 15px;
        top: 15px;
        position: absolute
    }
    
    .popup-overlay.default .slideshow-container .carousel-item .image-text .description {
        display: -webkit-box;
        -webkit-box-orient: vertical;
        -webkit-line-clamp: 2
    }
    
    .popup-overlay.default .slideshow-container .carousel-item .image-text .description:hover {
        max-height: 100%;
        display: block
    }
    
    .popup-overlay.default .close-button {
        width: 17px;
        height: 17px;
        padding: 10px;
        right: 20px;
        top: 20px;
        font-size: 17px
    }
    
    .popup-overlay.default .close-button .close-button-background {
        display: none;
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=10)";
        filter: alpha(opacity=10);
        -moz-opacity: .1;
        -khtml-opacity: .1;
        opacity: .1;
        zoom:1}
    
    .popup-overlay.default .close-button:hover .close-button-background {
        display: block
    }
    
    .popup-overlay.default .slideshow-container {
        top: 10%;
        bottom: 200px
    }
    
    .popup-overlay.default .slideshow-container .carousel-container .slideshow-carousel-container {
        margin: 0 24px
    }
    
    .popup-overlay.default .slideshow-container .carousel-item {
        z-index: 1
    }
    
    .popup-overlay.default .slideshow-container .carousel-item .image,.popup-overlay.default .slideshow-container .carousel-item .video {
        font-size: 0;
        text-align: center;
        white-space: nowrap
    }
    
    .popup-overlay.default .slideshow-container .carousel-item .image-text {
        position: absolute;
        width: 100%;
        left: 0;
        bottom: 0;
        white-space: normal;
        z-index: 1
    }
    
    .popup-overlay.default .slideshow-container .carousel-item .image-text .background {
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        z-index: -1
    }
    
    .popup-overlay.default .slideshow-container .carousel-item .image-text .title {
        font-size: 18px;
        font-weight: 700;
        padding: 0 120px 0 24px;
        margin-top: 12px;
        text-align: left;
        white-space: nowrap;
        overflow: hidden;
        text-overflow: ellipsis
    }
    
    .popup-overlay.default .slideshow-container .carousel-item .image-text .description {
        position: relative;
        font-size: 13px;
        padding: 0 120px 0 24px;
        margin: 9px 0 12px;
        text-align: left;
        line-height: 18px;
        max-height: 36px;
        overflow: hidden
    }
    
    .popup-overlay.default .slideshow-container .carousel-item .image-text .numbers-container {
        position: absolute;
        font-size: 16px;
        right: 24px;
        top: 14px
    }
    
    .popup-overlay.default .slideshow-container .carousel-item .image-text .link {
        position: relative;
        float: right;
        font-size: 13px;
        margin: -31px 24px 16px 0;
        color: #fff
    }
    
    .popup-overlay.default .slideshow-container .carousel-item .video .video-container .play-button {
        width: 90px;
        height: 90px;
        margin: -45px 0 0 -45px;
        font-size: 70px;
        background: #000;
        color: #fff;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=60)";
        filter: alpha(opacity=60);
        -moz-opacity: .6;
        -khtml-opacity: .6;
        opacity: .6;
        zoom:1;transition: opacity .1s
    }
    
    .popup-overlay.default .slideshow-container .carousel-item .video .video-container .play-button:before {
        margin-top: 10px
    }
    
    .popup-overlay.default .slideshow-container .carousel-item .video:hover .video-container .play-button {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=80)";
        filter: alpha(opacity=80);
        -moz-opacity: .8;
        -khtml-opacity: .8;
        opacity: .8;
        zoom:1}
    
    .popup-overlay.default .slideshow-container .carousel-item.current {
        z-index: 1
    }
    
    .popup-overlay.default .slideshow-container .carousel-item .no-title .image-text .title {
        display: none
    }
    
    .popup-overlay.default .slideshow-container .carousel-item .no-title .image-text .description {
        margin-top: 13px
    }
    
    .popup-overlay.default .slideshow-container .carousel-item .no-description .image-text .title {
        margin-bottom: 12px
    }
    
    .popup-overlay.default .slideshow-container .carousel-item .no-description .image-text .description {
        display: none
    }
    
    .popup-overlay.default .slideshow-container .carousel-item .no-description .image-text .link {
        margin-top: -4px
    }
    
    .popup-overlay.default .slideshow-container .carousel-item .no-title.no-description .image-text {
        height: 47px
    }
    
    .popup-overlay.default .slideshow-container .carousel-item .no-title.no-description .link {
        float: left;
        margin: 16px 24px
    }
    
    .popup-overlay.default .slideshow-container .carousel-item .no-link .image-text .link,.popup-overlay.default .slideshow-container .carousel-item.state-loading .image-text {
        display: none
    }
    
    .popup-overlay.default .slideshow-container .navigation-button {
        width: 35px;
        height: 66px;
        padding: 20px;
        top: 50%;
        margin-top: -53px
    }
    
    .popup-overlay.default .slideshow-container .navigation-button .navigation-button-background {
        display: none;
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=10)";
        filter: alpha(opacity=10);
        -moz-opacity: .1;
        -khtml-opacity: .1;
        opacity: .1;
        zoom:1}
    
    .popup-overlay.default .slideshow-container .navigation-button:hover .navigation-button-background {
        display: block
    }
    
    .popup-overlay.default .slideshow-container .navigation-button.prev {
        left: 10px
    }
    
    .popup-overlay.default .slideshow-container .navigation-button.next {
        right: 10px
    }
    
    .popup-overlay.default .slideshow-container .navigation-button .icon-container {
        position: relative;
        font-size: 66px
    }
    
    .popup-overlay.default .footer {
        height: 134px
    }
    
    .popup-overlay.default .footer .thumbs-container {
        height: 110px;
        margin: 0 24px
    }
    
    .popup-overlay.default .footer .thumbs-container .thumb .image-thumb {
        width: 166px;
        height: 110px;
        margin: 0 7px
    }
    
    @media (max-width: 1024px) {
        .popup-overlay.default .close-button {
            right:2px;
            top: 2px
        }
    
        .popup-overlay.default .popup-header {
            height: 40px
        }
    
        .popup-overlay.default .slideshow-container {
            top: 40px;
            bottom: 120px
        }
    
        .popup-overlay.default .footer {
            height: 100px
        }
    
        .popup-overlay.default .footer .thumbs-container {
            height: 80px;
            margin: 0 20px
        }
    
        .popup-overlay.default .footer .thumbs-container .thumb .image-thumb {
            width: 120px;
            height: 80px;
            margin: 0 5px
        }
    }
    
    @media (max-height: 580px) {
        .popup-overlay.default .close-button {
            right:2px;
            top: 2px
        }
    
        .popup-overlay.default .popup-header {
            height: 20px
        }
    
        .popup-overlay.default .slideshow-container {
            top: 20px;
            bottom: 20px
        }
    
        .popup-overlay.default .footer {
            display: none
        }
    }
    
    .popup-overlay.default.no-thumbs .slideshow-container,.popup-overlay.default.single-item-popup .slideshow-container {
        bottom: 10%
    }
    
    .popup-overlay.default.no-thumbs .footer,.popup-overlay.default.no-title .carousel-item .image-text .title,.popup-overlay.default.single-item-popup .footer {
        display: none
    }
    
    .popup-overlay.default.no-title .carousel-item .image-text .description {
        margin-top: 13px
    }
    
    .popup-overlay.default.no-description .carousel-item .image-text .title {
        margin-bottom: 12px
    }
    
    .popup-overlay.default.no-description .carousel-item .image-text .description {
        display: none
    }
    
    .popup-overlay.default.no-description .carousel-item .image-text .link {
        margin-top: -4px
    }
    
    .popup-overlay.default.no-title.no-description .carousel-item .image-text {
        height: 47px
    }
    
    .popup-overlay.default.no-title.no-description .carousel-item .link {
        float: left;
        margin: 16px 24px
    }
    
    .popup-overlay.mobile-popup {
        font-family: 'Open Sans',sans-serif;
        -webkit-text-size-adjust: 100%
    }
    
    .popup-overlay.mobile-popup .popup-header {
        position: relative;
        height: 45px;
        color: #fff;
        font-size: 11px;
        box-shadow: 0 1px 0 0 rgba(255,255,255,.1);
        z-index: 11
    }
    
    .popup-overlay.mobile-popup .popup-header .separator {
        float: left;
        width: 1px;
        height: 45px;
        margin: 0 10px;
        background: rgba(255,255,255,.1)
    }
    
    .popup-overlay.mobile-popup .popup-header .separator.float-right {
        float: right
    }
    
    .popup-overlay.mobile-popup .popup-header .thumbs-toggle {
        float: left;
        width: 24px;
        height: 24px;
        margin: 10px 0 0 10px;
        font-size: 24px;
        cursor: pointer
    }
    
    .popup-overlay.mobile-popup .popup-header .navigation-button {
        position: relative;
        float: left;
        width: 24px;
        height: 24px;
        margin-top: 10px;
        font-size: 20px
    }
    
    .popup-overlay.mobile-popup .popup-header .navigation-button .icon-container {
        position: absolute;
        left: 2px;
        top: 2px
    }
    
    .popup-overlay.mobile-popup .popup-header .numbers {
        float: left;
        min-width: 35px;
        margin-top: 14px;
        text-align: center
    }
    
    .popup-overlay.mobile-popup .popup-header .header-title {
        padding: 14px 10px 0;
        text-transform: uppercase;
        white-space: nowrap;
        overflow: hidden;
        text-overflow: ellipsis
    }
    
    .popup-overlay.mobile-popup .popup-header .close-button {
        position: relative;
        float: right;
        width: 24px;
        height: 24px;
        margin: 10px 10px 0 0;
        font-size: 14px
    }
    
    .popup-overlay.mobile-popup .popup-header .close-button:before {
        position: absolute;
        left: 5px;
        top: 5px
    }
    
    .popup-overlay.mobile-popup .footer {
        position: absolute;
        width: 100%;
        height: auto;
        top: 45px;
        bottom: 1000px;
        overflow: hidden;
        background: rgba(0,0,0,.8);
        z-index: 10;
        transition: bottom .3s
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container {
        height: 100%;
        margin: 0;
        text-align: left;
        overflow: auto
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .slideshow-thumbs-container {
        width: 100%;
        height: auto
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .slideshow-thumbs-container .slideshow-thumbs-content {
        width: 100%
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .slideshow-thumbs-container .thumbs {
        height: auto;
        padding: 20px 0 0;
        white-space: normal
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .thumb {
        width: 100%
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .thumb .image-thumb {
        position: relative;
        width: 100%;
        min-height: 110px;
        margin: 0;
        opacity: .8
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .thumb .image-thumb .image {
        float: left;
        width: 76px;
        height: 76px;
        margin-left: 20px;
        border: 2px solid #fff
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .thumb .image-thumb .thumb-text {
        margin: 10px 20px 30px 115px;
        color: #fff;
        font-size: 13px
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .thumb .image-thumb .thumb-text .title {
        font-weight: 600;
        text-transform: uppercase;
        white-space: nowrap;
        text-overflow: ellipsis;
        overflow: hidden
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .thumb .image-thumb .thumb-text .description {
        max-height: 34px;
        margin-top: 9px;
        font-size: 11px;
        line-height: 17px;
        color: #d0d0d0;
        overflow: hidden
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .thumb .image-thumb .thumb-text .show-more {
        display: none;
        position: relative;
        padding: 8px 10px 10px 15px;
        margin-bottom: -10px;
        font-size: 8px;
        color: #b0b0b0;
        text-transform: uppercase
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .thumb .image-thumb .thumb-text .show-more .icon {
        position: absolute;
        left: 0;
        top: 6px;
        font-size: 15px
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .thumb .image-thumb .thumb-full-text {
        display: none;
        margin: 10px 20px 30px 115px;
        color: #fff;
        font-size: 13px
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .thumb .image-thumb .thumb-full-text .title {
        font-weight: 600;
        text-transform: uppercase
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .thumb .image-thumb .thumb-full-text .description {
        margin-top: 9px;
        font-size: 11px;
        line-height: 17px;
        color: #d0d0d0
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .thumb .image-thumb .thumb-full-text .show-less {
        position: relative;
        display: inline-block;
        padding: 8px 10px 10px 15px;
        margin-bottom: -10px;
        font-size: 8px;
        color: #b0b0b0;
        text-transform: uppercase
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .thumb .image-thumb .thumb-full-text .show-less .icon {
        position: absolute;
        left: 0;
        top: 6px;
        font-size: 15px
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .thumb .image-thumb .separator {
        position: absolute;
        height: 1px;
        left: 20px;
        right: 20px;
        bottom: 15px;
        background: rgba(255,255,255,.15)
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .thumb .image-thumb.has-long-text .show-more {
        display: inline-block
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .thumb .image-thumb.has-long-text.show-full-text .thumb-text {
        display: none
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .thumb .image-thumb.has-long-text.show-full-text .thumb-full-text {
        display: block
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .thumb:last-child .image-thumb {
        height: 80px
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .thumb:last-child .separator {
        display: none
    }
    
    .popup-overlay.mobile-popup .footer .thumbs-container .thumb.current .image-thumb {
        opacity: 1;
        filter: alpha(opacity=100)
    }
    
    .popup-overlay.mobile-popup .footer .scrolling-view,.popup-overlay.mobile-popup .footer .scrolling-view .scrollable-pane {
        height: 100%
    }
    
    .popup-overlay.mobile-popup .footer .scrolling-view .scrollbar-2.vertical {
        width: 5px
    }
    
    .popup-overlay.mobile-popup .footer .scrolling-view .scrollbar-2.vertical .scrollbar-handle {
        background: rgba(255,255,255,.2)
    }
    
    .popup-overlay.mobile-popup .footer .scrolling-view .scrollbar-2.state-active .slide-area {
        background: inherit
    }
    
    .popup-overlay.mobile-popup .footer .scrolling-view .scrollbar-2:hover .slide-area {
        background: rgba(255,255,255,.1)
    }
    
    .popup-overlay.mobile-popup .footer .scrolling-view .scrollbar-2:hover .scrollbar-handle {
        background: inherit
    }
    
    .popup-overlay.mobile-popup .footer.visible {
        bottom: 0
    }
    
    .popup-overlay.mobile-popup .slideshow-container {
        top: 45px;
        bottom: 0
    }
    
    .popup-overlay.mobile-popup .slideshow-container .carousel-item .video {
        width: 100%;
        height: 100%;
        left: 0;
        top: 0;
        background: center no-repeat;
        background-size: cover
    }
    
    .popup-overlay.mobile-popup .slideshow-container .carousel-item .video img {
        visibility: hidden
    }
    
    .popup-overlay.mobile-popup .slideshow-container .item-link {
        visibility: visible;
        position: absolute;
        width: 30px;
        height: 30px;
        right: 10px;
        bottom: 10px;
        font-size: 20px;
        color: #fff;
        background: rgba(0,0,0,.5);
        border: 1px solid rgba(255,255,255,.1);
        z-index: 5;
        opacity: 0
    }
    
    .popup-overlay.mobile-popup .slideshow-container .item-link:before {
        position: absolute;
        left: 5px;
        top: 5px
    }
    
    .popup-overlay.mobile-popup .slideshow-container .item-link.has-link.visible {
        visibility: visible;
        opacity: 1;
        transition: opacity .3s
    }
    
    .popup-overlay.mobile-popup.single-item-popup .popup-header .navigation-controls,.popup-overlay.mobile-popup.video-popup .slideshow-container .item-link {
        display: none
    }
    
    .popup-overlay.popup-1 .close-button {
        width: 17px;
        height: 17px;
        right: 30px;
        top: 30px;
        font-size: 17px;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=80)";
        filter: alpha(opacity=80);
        -moz-opacity: .8;
        -khtml-opacity: .8;
        opacity: .8;
        zoom:1}
    
    .popup-overlay.popup-1 .close-button:hover {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
        filter: alpha(opacity=100);
        -moz-opacity: 1;
        -khtml-opacity: 1;
        opacity: 1;
        zoom:1}
    
    .popup-overlay.popup-1 .popup-text-sidebar {
        position: absolute;
        width: 360px;
        height: 100%;
        right: 0;
        top: 0
    }
    
    .popup-overlay.popup-1 .popup-text-sidebar .social-share-links {
        display: none;
        position: absolute;
        left: 26px;
        top: 21px
    }
    
    .popup-overlay.popup-1 .popup-text-sidebar .social-share-links .share-link {
        float: left;
        position: relative;
        width: 34px;
        height: 34px;
        margin-right: 7px;
        font-size: 30px;
        text-decoration: none
    }
    
    .popup-overlay.popup-1 .popup-text-sidebar .social-share-links .share-link .share-link-background {
        position: absolute;
        width: 30px;
        height: 30px;
        left: 0;
        top: 0;
        border: 2px solid;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=50)";
        filter: alpha(opacity=50);
        -moz-opacity: .5;
        -khtml-opacity: .5;
        opacity: .5;
        zoom:1;border-radius: 20px
    }
    
    .popup-overlay.popup-1 .popup-text-sidebar .social-share-links .share-link .share-link-icon {
        position: absolute;
        left: 7px;
        top: 7px;
        font-size: 20px;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=80)";
        filter: alpha(opacity=80);
        -moz-opacity: .8;
        -khtml-opacity: .8;
        opacity: .8;
        zoom:1}
    
    .popup-overlay.popup-1 .popup-text-sidebar .social-share-links .share-link:hover .share-link-background {
        background: rgba(0,0,0,.1)
    }
    
    .popup-overlay.popup-1 .popup-text-sidebar .social-share-links .share-link:hover .share-link-icon {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
        filter: alpha(opacity=100);
        -moz-opacity: 1;
        -khtml-opacity: 1;
        opacity: 1;
        zoom:1}
    
    .popup-overlay.popup-1 .popup-text-sidebar .item-text {
        position: absolute;
        left: 26px;
        right: 26px;
        top: 110px;
        bottom: 26px;
        font-size: 14px;
        word-wrap: break-word
    }
    
    .popup-overlay.popup-1 .popup-text-sidebar .item-text .numbers-container {
        margin-bottom: 15px
    }
    
    .popup-overlay.popup-1 .popup-text-sidebar .item-text .scrollable-text {
        position: absolute;
        width: 100%;
        top: 34px;
        bottom: 0
    }
    
    .popup-overlay.popup-1 .popup-text-sidebar .item-text .title {
        padding-bottom: 20px;
        font-size: 24px;
        font-weight: 700
    }
    
    .popup-overlay.popup-1 .popup-text-sidebar .item-text .separator {
        border-bottom: 1px solid #fff;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=50)";
        filter: alpha(opacity=50);
        -moz-opacity: .5;
        -khtml-opacity: .5;
        opacity: .5;
        zoom:1}
    
    .popup-overlay.popup-1 .popup-text-sidebar .item-text .description {
        margin: 20px 0 15px;
        line-height: 20px
    }
    
    .popup-overlay.popup-1 .popup-text-sidebar .item-text .scrolling-view,.popup-overlay.popup-1 .popup-text-sidebar .item-text .scrolling-view .scrolling-pane {
        height: 100%
    }
    
    .popup-overlay.popup-1 .popup-text-sidebar .item-text .scrolling-view .scrollbar {
        right: -18px
    }
    
    .popup-overlay.popup-1 .popup-text-sidebar .item-text.no-description .description,.popup-overlay.popup-1 .popup-text-sidebar .item-text.no-link .link,.popup-overlay.popup-1 .popup-text-sidebar .item-text.no-title .title {
        display: none
    }
    
    .popup-overlay.popup-1 .popup-text-sidebar .item-text.no-link .description {
        margin-bottom: 0
    }
    
    .popup-overlay.popup-1 .slideshow-container {
        left: 0;
        right: 360px;
        top: 0;
        bottom: 108px;
        padding: 35px 35px 28px
    }
    
    .popup-overlay.popup-1 .slideshow-container .carousel-container .slideshow-carousel-container {
        margin: 0
    }
    
    .popup-overlay.popup-1 .slideshow-container .carousel-container .video .video-container .play-button {
        width: 90px;
        height: 90px;
        margin: -45px 0 0 -45px;
        font-size: 70px;
        background: #000;
        color: #fff;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=60)";
        filter: alpha(opacity=60);
        -moz-opacity: .6;
        -khtml-opacity: .6;
        opacity: .6;
        zoom:1;transition: opacity .1s
    }
    
    .popup-overlay.popup-1 .slideshow-container .carousel-container .video .video-container .play-button:before {
        margin-top: 10px
    }
    
    .popup-overlay.popup-1 .slideshow-container .carousel-container .video:hover .video-container .play-button {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=80)";
        filter: alpha(opacity=80);
        -moz-opacity: .8;
        -khtml-opacity: .8;
        opacity: .8;
        zoom:1}
    
    .popup-overlay.popup-1 .slideshow-container .navigation-button {
        width: 35px;
        height: 66px;
        padding: 20px;
        top: 50%;
        margin-top: -53px
    }
    
    .popup-overlay.popup-1 .slideshow-container .navigation-button .navigation-button-background {
        display: none;
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=20)";
        filter: alpha(opacity=20);
        -moz-opacity: .2;
        -khtml-opacity: .2;
        opacity: .2;
        zoom:1}
    
    .popup-overlay.popup-1 .slideshow-container .navigation-button:hover .navigation-button-background {
        display: block
    }
    
    .popup-overlay.popup-1.no-thumbs .footer,.popup-overlay.popup-1.single-item-popup .footer {
        display: none
    }
    
    .popup-overlay.popup-1 .slideshow-container .navigation-button.prev {
        left: 10px
    }
    
    .popup-overlay.popup-1 .slideshow-container .navigation-button.next {
        right: 10px
    }
    
    .popup-overlay.popup-1 .slideshow-container .navigation-button .icon-container {
        position: relative;
        font-size: 66px
    }
    
    .popup-overlay.popup-1 .footer {
        height: 108px;
        left: 36px;
        right: 396px
    }
    
    .popup-overlay.popup-1 .footer .thumbs-container {
        height: 73px;
        margin: 0 auto;
        min-width: 300px
    }
    
    .popup-overlay.popup-1 .footer .thumbs-container .thumb .image-thumb {
        width: 110px;
        height: 73px;
        margin: 0 5px
    }
    
    .popup-overlay.popup-1 .footer .thumbs-container .thumb:first-child .image-thumb {
        margin-left: 0
    }
    
    .popup-overlay.popup-1 .footer .thumbs-container .thumb:last-child .image-thumb {
        margin-right: 0
    }
    
    .popup-overlay.popup-1.single-item-popup .popup-text-sidebar .item-text .scrollable-text {
        top: 0
    }
    
    .popup-overlay.popup-1.single-item-popup .slideshow-container {
        bottom: 0
    }
    
    .popup-overlay.popup-1.no-thumbs .slideshow-container {
        bottom: 0
    }
    
    .popup-overlay.popup-1.show-share-buttons .popup-text-sidebar .social-share-links.has-share-link {
        display: block
    }
    
    .popup-overlay.popup-1.video-popup .slideshow-container .navigation-button {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=0)";
        filter: alpha(opacity=0);
        -moz-opacity: 0;
        -khtml-opacity: 0;
        opacity: 0;
        zoom:1;transition: opacity .2s
    }
    
    .popup-overlay.popup-1.video-popup .slideshow-container:hover .navigation-button {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
        filter: alpha(opacity=100);
        -moz-opacity: 1;
        -khtml-opacity: 1;
        opacity: 1;
        zoom:1}
    
    .popup-overlay.popup-2 {
        position: absolute;
        left: 0;
        right: 0;
        top: 0;
        bottom: 0
    }
    
    .popup-overlay.popup-2 .close-button {
        width: 14px;
        height: 14px;
        right: 20px;
        top: 20px;
        padding: 2px;
        font-size: 14px;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=55.00000000000001)";
        filter: alpha(opacity=55.00000000000001);
        -moz-opacity: .55;
        -khtml-opacity: .55;
        opacity: .55;
        zoom:1}
    
    .popup-overlay.popup-2 .separator {
        border-bottom: 1px solid;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=20)";
        filter: alpha(opacity=20);
        -moz-opacity: .2;
        -khtml-opacity: .2;
        opacity: .2;
        zoom:1}
    
    .popup-overlay.popup-2 .popup-text-sidebar {
        position: absolute;
        width: 350px;
        height: 100%;
        right: 0;
        top: 0
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .social-share-links {
        display: none;
        position: absolute;
        left: 26px;
        top: 26px
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .social-share-links .share-link {
        float: left;
        position: relative;
        width: 30px;
        height: 30px;
        margin-right: 5px;
        font-size: 30px;
        text-decoration: none
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .social-share-links .share-link span {
        position: absolute;
        left: 8px;
        top: 8px;
        font-size: 14px;
        color: #fff
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .social-share-links .share-link.facebook {
        color: #496eb5
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .social-share-links .share-link.twitter {
        color: #69c8ed
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .social-share-links .share-link.pinterest {
        color: #ef4646
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .social-share-links .share-link:hover {
        width: 34px;
        height: 34px;
        margin: -2px 3px 0 -2px;
        font-size: 34px
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .social-share-links .share-link:hover span {
        font-size: 18px
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .item-text {
        height: 142px;
        padding: 80px 26px 0;
        font-size: 14px;
        font-family: 'Open Sans',sans-serif;
        overflow: hidden;
        word-wrap: break-word
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .item-text .item-text-inner {
        position: relative
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .item-text .numbers-container {
        margin-bottom: 15px
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .item-text .title {
        max-height: 48px;
        font-size: 18px;
        line-height: 24px
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .item-text .description {
        padding-top: 16px;
        line-height: 20px;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=70)";
        filter: alpha(opacity=70);
        -moz-opacity: .7;
        -khtml-opacity: .7;
        opacity: .7;
        zoom:1}
    
    .popup-overlay.popup-2 .popup-text-sidebar .item-text .description:empty {
        display: none
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .item-text .link {
        position: relative;
        display: inline-block;
        padding-left: 23px;
        margin: 12px 0;
        line-height: 14px;
        text-decoration: none
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .item-text .link:hover {
        text-decoration: underline
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .item-text .link span {
        position: absolute;
        left: 0;
        top: -5px;
        font-size: 20px;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=50)";
        filter: alpha(opacity=50);
        -moz-opacity: .5;
        -khtml-opacity: .5;
        opacity: .5;
        zoom:1}
    
    .popup-overlay.popup-2 .popup-text-sidebar .item-text .read-more {
        display: none;
        position: relative;
        padding-right: 4px;
        cursor: pointer
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .item-text .read-more .chevron {
        float: right;
        margin-top: 4px
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .item-text.no-link .title {
        max-height: 72px;
        padding-bottom: 12px
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .item-text.no-link .link {
        display: none
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .item-text.long-text {
        height: 180px
    }
    
    .popup-overlay.popup-2 .popup-text-sidebar .item-text.long-text .read-more {
        display: inline-block
    }
    
    .popup-overlay.popup-2 .footer {
        height: auto;
        top: 260px;
        bottom: 25px
    }
    
    .popup-overlay.popup-2 .footer .full-item-text {
        display: none;
        width: 298px;
        margin: 0 26px 26px;
        font-size: 14px;
        font-family: 'Open Sans',sans-serif;
        word-wrap: break-word
    }
    
    .popup-overlay.popup-2 .footer .full-item-text .title {
        font-size: 18px;
        line-height: 24px
    }
    
    .popup-overlay.popup-2 .footer .full-item-text .description {
        padding-top: 16px;
        line-height: 20px;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=70)";
        filter: alpha(opacity=70);
        -moz-opacity: .7;
        -khtml-opacity: .7;
        opacity: .7;
        zoom:1}
    
    .popup-overlay.popup-2 .footer .full-item-text .link {
        position: relative;
        display: inline-block;
        padding-left: 23px;
        margin: 12px 0;
        line-height: 14px;
        text-decoration: none
    }
    
    .popup-overlay.popup-2 .footer .full-item-text .link span {
        position: absolute;
        left: 0;
        top: -5px;
        font-size: 20px;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=50)";
        filter: alpha(opacity=50);
        -moz-opacity: .5;
        -khtml-opacity: .5;
        opacity: .5;
        zoom:1}
    
    .popup-overlay.popup-2 .footer .full-item-text .read-less {
        position: relative;
        display: inline-block;
        padding-right: 4px;
        cursor: pointer
    }
    
    .popup-overlay.popup-2 .footer .full-item-text.no-link .link,.popup-overlay.popup-2.show-full-text .footer .short-text-separator,.popup-overlay.popup-2.show-full-text .popup-text-sidebar .item-text {
        display: none
    }
    
    .popup-overlay.popup-2 .footer .full-item-text .read-less .chevron {
        float: right;
        margin-top: 4px
    }
    
    .popup-overlay.popup-2 .footer .full-item-text .long-text-separator {
        height: 26px
    }
    
    .popup-overlay.popup-2 .footer .full-item-text.no-link .title {
        padding-bottom: 12px
    }
    
    .popup-overlay.popup-2 .footer .short-text-separator {
        margin: 0 26px 20px
    }
    
    .popup-overlay.popup-2 .footer .thumbs-scroller-container {
        position: absolute;
        width: 100%;
        top: 21px;
        bottom: 0
    }
    
    .popup-overlay.popup-2 .footer .thumbs-scroller-container-inner {
        position: absolute;
        top: 0;
        bottom: 0
    }
    
    .popup-overlay.popup-2 .footer .thumbs-container {
        height: auto;
        bottom: 0;
        margin: 0 17px
    }
    
    .popup-overlay.popup-2 .footer .thumbs-container .slideshow-thumbs-container {
        height: auto
    }
    
    .popup-overlay.popup-2 .footer .thumbs-container .slideshow-thumbs-container .thumbs {
        height: auto;
        white-space: normal;
        text-align: left
    }
    
    .popup-overlay.popup-2 .footer .thumbs-container .thumb {
        width: 158px;
        height: 106px
    }
    
    .popup-overlay.popup-2 .footer .thumbs-container .thumb .image-thumb {
        width: 140px;
        height: 88px;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
        filter: alpha(opacity=100);
        -moz-opacity: 1;
        -khtml-opacity: 1;
        opacity: 1;
        zoom:1;margin: 0 9px 18px
    }
    
    .popup-overlay.popup-2 .footer .thumbs-container .thumb .image-thumb .image {
        width: 140px;
        height: 88px
    }
    
    .popup-overlay.popup-2 .footer .thumbs-container .thumb .image-thumb .current-cover {
        width: 128px;
        height: 76px;
        left: 0;
        top: 0;
        border: 6px solid
    }
    
    .popup-overlay.popup-2 .footer .thumbs-container .thumb .image-thumb .current-cover .current-cover-border {
        position: absolute;
        width: 138px;
        height: 86px;
        left: -6px;
        top: -6px;
        border: 1px solid;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=20)";
        filter: alpha(opacity=20);
        -moz-opacity: .2;
        -khtml-opacity: .2;
        opacity: .2;
        zoom:1}
    
    .popup-overlay.popup-2 .footer .thumbs-container .thumb:last-child,.popup-overlay.popup-2 .footer .thumbs-container .thumb:nth-last-child(2) {
        height: 88px
    }
    
    .popup-overlay.popup-2 .footer .thumbs-container .thumb .image-thumb:hover img {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=90)";
        filter: alpha(opacity=90);
        -moz-opacity: .9;
        -khtml-opacity: .9;
        opacity: .9;
        zoom:1}
    
    .popup-overlay.popup-2 .footer .thumbs-container .thumb:last-child .image-thumb {
        margin: 0 9px
    }
    
    .popup-overlay.popup-2 .footer .thumbs-container .thumb:nth-last-child(2) .image-thumb {
        margin-bottom: 0
    }
    
    .popup-overlay.popup-2 .footer .thumbs-container .thumb.current .image-thumb {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
        filter: alpha(opacity=100);
        -moz-opacity: 1;
        -khtml-opacity: 1;
        opacity: 1;
        zoom:1}
    
    .popup-overlay.popup-2 .footer .scrolling-view,.popup-overlay.popup-2 .footer .scrolling-view .scrolling-pane {
        height: 100%
    }
    
    .popup-overlay.popup-2 .footer .scrolling-view .scrollbar {
        right: 10px
    }
    
    .popup-overlay.popup-2 .slideshow-container {
        right: 350px;
        top: 0;
        bottom: 0;
        padding: 50px
    }
    
    .popup-overlay.popup-2 .slideshow-container .carousel-container .slideshow-carousel-container {
        margin: 0
    }
    
    .popup-overlay.popup-2 .slideshow-container .carousel-container .video .video-container .play-button {
        width: 90px;
        height: 90px;
        margin: -45px 0 0 -45px;
        font-size: 70px;
        background: #000;
        color: #fff;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=60)";
        filter: alpha(opacity=60);
        -moz-opacity: .6;
        -khtml-opacity: .6;
        opacity: .6;
        zoom:1;transition: opacity .1s
    }
    
    .popup-overlay.popup-2 .slideshow-container .carousel-container .video .video-container .play-button:before {
        margin-top: 10px
    }
    
    .popup-overlay.popup-2 .slideshow-container .carousel-container .video:hover .video-container .play-button {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=80)";
        filter: alpha(opacity=80);
        -moz-opacity: .8;
        -khtml-opacity: .8;
        opacity: .8;
        zoom:1}
    
    .popup-overlay.popup-2 .slideshow-container .navigation-button {
        width: 70px;
        height: 70px;
        top: 50%;
        margin-top: -35px;
        color: #fff
    }
    
    .popup-overlay.popup-2 .slideshow-container .navigation-button .navigation-button-background {
        position: absolute;
        width: 100%;
        height: 100%;
        left: 0;
        top: 0;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=20)";
        filter: alpha(opacity=20);
        -moz-opacity: .2;
        -khtml-opacity: .2;
        opacity: .2;
        zoom:1;transition: opacity .1s
    }
    
    .popup-overlay.popup-2 .slideshow-container .navigation-button .icon-container {
        text-align: center;
        margin-top: 23px;
        font-size: 24px;
        font-weight: 700
    }
    
    .popup-overlay.popup-2 .slideshow-container .navigation-button.prev {
        left: 20px
    }
    
    .popup-overlay.popup-2 .slideshow-container .navigation-button.next {
        right: 20px
    }
    
    .popup-overlay.popup-2 .slideshow-container .navigation-button:hover .navigation-button-background {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=30)";
        filter: alpha(opacity=30);
        -moz-opacity: .3;
        -khtml-opacity: .3;
        opacity: .3;
        zoom:1}
    
    .popup-overlay.popup-2.show-full-text .footer {
        top: 80px
    }
    
    .popup-overlay.popup-2.show-full-text .footer .thumbs-scroller-container {
        top: 0
    }
    
    .popup-overlay.popup-2.show-full-text .footer .full-item-text {
        display: block
    }
    
    .popup-overlay.popup-2.no-thumbs .footer .short-text-separator,.popup-overlay.popup-2.no-thumbs .popup-text-sidebar .item-text,.popup-overlay.popup-2.single-item-popup .footer .short-text-separator,.popup-overlay.popup-2.single-item-popup .popup-text-sidebar .item-text {
        display: none
    }
    
    .popup-overlay.popup-2.no-thumbs .footer,.popup-overlay.popup-2.single-item-popup .footer {
        top: 80px
    }
    
    .popup-overlay.popup-2.no-thumbs .footer .full-item-text,.popup-overlay.popup-2.single-item-popup .footer .full-item-text {
        display: block;
        border-bottom: none;
        padding-bottom: 0;
        margin-bottom: 0
    }
    
    .popup-overlay.popup-2.no-thumbs .footer .full-item-text .read-less,.popup-overlay.popup-2.no-thumbs .footer .thumbs-container,.popup-overlay.popup-2.single-item-popup .footer .full-item-text .read-less,.popup-overlay.popup-2.single-item-popup .footer .thumbs-container {
        display: none
    }
    
    .popup-overlay.popup-2.show-share-buttons .popup-text-sidebar .social-share-links.has-share-link {
        display: block
    }
    
    .popup-overlay.popup-2.video-popup .slideshow-container .navigation-button {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=0)";
        filter: alpha(opacity=0);
        -moz-opacity: 0;
        -khtml-opacity: 0;
        opacity: 0;
        zoom:1;transition: opacity .2s
    }
    
    .popup-overlay.popup-2.video-popup .slideshow-container:hover .navigation-button {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
        filter: alpha(opacity=100);
        -moz-opacity: 1;
        -khtml-opacity: 1;
        opacity: 1;
        zoom:1}
    
    .popup-overlay.popup-3 .header {
        position: absolute;
        right: 30px;
        top: 30px;
        z-index: 30
    }
    
    .popup-overlay.popup-3 .header .close-button {
        position: static;
        float: right;
        width: 17px;
        height: 17px;
        font-size: 17px
    }
    
    .popup-overlay.popup-3 .header .close-button:hover {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=80)";
        filter: alpha(opacity=80);
        -moz-opacity: .8;
        -khtml-opacity: .8;
        opacity: .8;
        zoom:1}
    
    .popup-overlay.popup-3 .header .numbers-container {
        float: right;
        margin: -5px 20px 0;
        padding: 0 25px;
        border-left: 1px solid;
        border-right: 1px solid;
        font-size: 16px;
        line-height: 28px;
        font-family: 'Open Sans',sans-serif
    }
    
    .popup-overlay.popup-3 .header .numbers-container .numbers-separator {
        margin: 0 5px;
        font-style: italic
    }
    
    .popup-overlay.popup-3 .header .thumbs-toggle {
        float: right;
        width: 17px;
        height: 17px;
        font-size: 17px;
        cursor: pointer
    }
    
    .popup-overlay.popup-3 .header .thumbs-toggle:hover {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=80)";
        filter: alpha(opacity=80);
        -moz-opacity: .8;
        -khtml-opacity: .8;
        opacity: .8;
        zoom:1}
    
    .popup-overlay.popup-3 .slideshow-container {
        left: 0;
        right: 0;
        top: 0;
        bottom: 0;
        margin: 80px 0 70px
    }
    
    .popup-overlay.popup-3 .slideshow-container .carousel-container .slideshow-carousel-container {
        margin: 0
    }
    
    .popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item {
        display: none;
        width: auto;
        height: auto;
        left: 230px;
        right: 230px;
        top: 0;
        bottom: 130px
    }
    
    .popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item .image,.popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item .video {
        position: absolute
    }
    
    .popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item .image img,.popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item .video img {
        display: block;
        width: 100%;
        height: 100%;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=50)";
        filter: alpha(opacity=50);
        -moz-opacity: .5;
        -khtml-opacity: .5;
        opacity: .5;
        zoom:1;transition: opacity .5s
    }
    
    .popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item .image img.hover,.popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item .video img.hover {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=70)";
        filter: alpha(opacity=70);
        -moz-opacity: .7;
        -khtml-opacity: .7;
        opacity: .7;
        zoom:1;transition: opacity .3s
    }
    
    .popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item .video .video-container .play-button {
        width: 80px;
        height: 80px;
        border: 5px solid #fff;
        margin: -45px 0 0 -45px;
        font-size: 60px;
        background: rgba(0,0,0,.6);
        color: #fff;
        border-radius: 50px;
        box-shadow: 0 0 10px rgba(0,0,0,.3);
        transition: all .1s
    }
    
    .popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item .video .video-container .play-button:before {
        margin-top: 10px
    }
    
    .popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item .video .video-container:hover .play-button {
        background: rgba(0,0,0,.8);
        -moz-transform: scale(1.1);
        -webkit-transform: scale(1.1);
        -ms-transform: scale(1.1);
        transform: scale(1.1)
    }
    
    .popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item .image-text-outer {
        position: absolute;
        width: 100%;
        bottom: -156px
    }
    
    .popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item .image-text-inner {
        position: relative;
        float: right;
        right: 50%
    }
    
    .popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item .image-text {
        position: relative;
        width: 100%;
        height: 130px;
        right: -50%;
        min-width: 300px;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=0)";
        filter: alpha(opacity=0);
        -moz-opacity: 0;
        -khtml-opacity: 0;
        opacity: 0;
        zoom:1;transition: opacity .4s
    }
    
    .popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item .image-text .title {
        font-size: 24px;
        line-height: 32px;
        font-weight: 700;
        margin-top: 26px;
        text-align: left;
        white-space: nowrap;
        overflow: hidden;
        text-overflow: ellipsis
    }
    
    .popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item .image-text .description {
        font-size: 13px;
        margin-top: 10px;
        text-align: left;
        line-height: 18px;
        max-height: 36px;
        overflow: hidden;
        display: -webkit-box;
        -webkit-box-orient: vertical;
        -webkit-line-clamp: 2
    }
    
    .popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item .image-text .description:hover {
        max-height: 100%;
        display: block
    }
    
    .popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item .image-text .link {
        display: inline-block;
        margin-top: 10px;
        font-size: 13px
    }
    
    .popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item .no-description .image-text .description,.popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item .no-link .image-text .link,.popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item .no-title .image-text .title,.popup-overlay.popup-3.no-description .slideshow-container .carousel-container .carousel-item .image-text .description,.popup-overlay.popup-3.no-title .slideshow-container .carousel-container .carousel-item .image-text .title,.popup-overlay.popup-3.single-item-popup .header .thumbs-toggle {
        display: none
    }
    
    .popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item.current {
        z-index: 2
    }
    
    .popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item.current .image img,.popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item.current .video img {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
        filter: alpha(opacity=100);
        -moz-opacity: 1;
        -khtml-opacity: 1;
        opacity: 1;
        zoom:1}
    
    .popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item.current .image-text {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
        filter: alpha(opacity=100);
        -moz-opacity: 1;
        -khtml-opacity: 1;
        opacity: 1;
        zoom:1;transition: opacity .5s .4s
    }
    
    .popup-overlay.popup-3 .slideshow-container .carousel-container .carousel-item .no-title .image-text .description {
        margin-top: 13px
    }
    
    .popup-overlay.popup-3 .slideshow-container .navigation-button {
        width: 130px;
        height: auto;
        top: 0;
        bottom: 120px;
        margin: 0
    }
    
    .popup-overlay.popup-3 .slideshow-container .navigation-button .icon-container {
        position: absolute;
        width: 130px;
        top: 50%;
        margin-top: -33px;
        text-align: center;
        font-size: 66px
    }
    
    .popup-overlay.popup-3 .slideshow-container .navigation-button.prev {
        left: 0
    }
    
    .popup-overlay.popup-3 .slideshow-container .navigation-button.next {
        right: 0
    }
    
    .popup-overlay.popup-3 .footer {
        height: 108px;
        left: 0;
        top: -188px;
        bottom: auto;
        padding-top: 80px;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=0)";
        filter: alpha(opacity=0);
        -moz-opacity: 0;
        -khtml-opacity: 0;
        opacity: 0;
        zoom:1;z-index: 20
    }
    
    .popup-overlay.popup-3 .footer .thumbs-container {
        height: 73px;
        margin: 0
    }
    
    .popup-overlay.popup-3 .footer .thumbs-container .thumb .image-thumb {
        width: 110px;
        height: 73px;
        margin: 0 5px
    }
    
    .popup-overlay.popup-3.single-item-popup .header .numbers-container {
        border-left: none
    }
    
    .popup-overlay.popup-3.no-title .slideshow-container .navigation-button {
        bottom: 98px
    }
    
    .popup-overlay.popup-3.no-title .slideshow-container .carousel-container .carousel-item {
        bottom: 102px
    }
    
    .popup-overlay.popup-3.no-title .slideshow-container .carousel-container .carousel-item .image-text .description {
        margin-top: 13px
    }
    
    .popup-overlay.popup-3.no-description .slideshow-container .navigation-button {
        bottom: 84px
    }
    
    .popup-overlay.popup-3.no-description .slideshow-container .carousel-container .carousel-item {
        bottom: 94px
    }
    
    .popup-overlay.popup-3.no-title.no-description .slideshow-container .navigation-button {
        bottom: 56px
    }
    
    .popup-overlay.popup-3.no-title.no-description .slideshow-container .carousel-container .carousel-item {
        bottom: 66px
    }
    
    .popup-overlay.popup-3.no-title.no-description .slideshow-container .carousel-container .carousel-item .image-text .link {
        margin-top: 5px
    }
    
    .popup-overlay.popup-4 {
        text-align: center;
        vertical-align: middle;
        white-space: nowrap;
        font-size: 0
    }
    
    .popup-overlay.popup-4 .close-button {
        width: 14px;
        height: 14px;
        right: 20px;
        top: 15px;
        padding: 1px;
        font-size: 14px;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=50)";
        filter: alpha(opacity=50);
        -moz-opacity: .5;
        -khtml-opacity: .5;
        opacity: .5;
        zoom:1}
    
    .popup-overlay.popup-4 .close-button:hover {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=60)";
        filter: alpha(opacity=60);
        -moz-opacity: .6;
        -khtml-opacity: .6;
        opacity: .6;
        zoom:1}
    
    .popup-overlay.popup-4 .popup-container {
        display: inline-block
    }
    
    .popup-overlay.popup-4 .popup-container-inner {
        position: relative;
        border-radius: 5px
    }
    
    .popup-overlay.popup-4 .slideshow-container {
        position: relative;
        left: 0;
        right: auto;
        top: 0;
        bottom: auto;
        padding: 40px 155px 20px 20px
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container {
        position: relative
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .slideshow-carousel-container {
        margin: 0
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item {
        display: none;
        width: 100%;
        height: 100%
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .image {
        position: absolute;
        min-width: 640px;
        min-height: 360px;
        font-size: 0;
        white-space: nowrap
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .image img {
        display: inline-block;
        width: auto;
        height: auto;
        max-width: 100%;
        max-height: 100%
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .video img {
        width: 100%;
        height: 100%
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .video .video-container .play-button {
        width: 80px;
        height: 80px;
        margin: -40px 0 0 -40px;
        font-size: 60px;
        background: #fff;
        color: #000;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=40)";
        filter: alpha(opacity=40);
        -moz-opacity: .4;
        -khtml-opacity: .4;
        opacity: .4;
        zoom:1;border-radius: 5px
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .video .video-container .play-button:before {
        margin-top: 10px
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .video .video-container iframe {
        position: relative;
        z-index: 2
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .video:hover .video-container .play-button {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=60)";
        filter: alpha(opacity=60);
        -moz-opacity: .6;
        -khtml-opacity: .6;
        opacity: .6;
        zoom:1}
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .image-text {
        position: absolute;
        width: 100%;
        bottom: 0;
        min-height: 65px;
        text-align: left;
        white-space: normal;
        z-index: 1
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .image-text .background {
        position: absolute;
        width: 100%;
        height: 100%;
        z-index: -1
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .image-text .title {
        font-size: 24px;
        font-weight: 100;
        margin: 16px 250px 0 24px;
        white-space: nowrap;
        overflow: hidden;
        text-overflow: ellipsis
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .image-text .description-wrapper {
        max-height: 0;
        overflow: hidden
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .image-text .description {
        font-size: 13px;
        margin: 10px 250px 16px 24px;
        line-height: 18px;
        max-height: 36px;
        overflow: hidden
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .shadow {
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        box-shadow: inset 0 0 7px rgba(0,0,0,.3);
        z-index: 1
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item.current .image-text .description-wrapper {
        transition: max-height .3s
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .no-title .image-text .description-wrapper,.popup-overlay.popup-4.no-title .slideshow-container .carousel-container .carousel-item .image-text .description-wrapper {
        transition: none;
        max-height: 62px
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .no-title .image-text .title {
        display: none
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .no-title .image-text .description {
        margin-top: 16px
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .no-description .image-text .title {
        margin-bottom: 16px
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .no-description .image-text .description,.popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .no-title.no-description .image-text {
        display: none
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .no-link .image-text .description,.popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item .no-link .image-text .title {
        margin-right: 24px
    }
    
    .popup-overlay.popup-4 .slideshow-container .carousel-container .carousel-item.state-loading .image-text {
        display: none
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner {
        position: relative;
        overflow: hidden
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner .social-share-links {
        display: none;
        position: absolute;
        right: 20px;
        top: 26px;
        z-index: 5
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner .social-share-links .share-link {
        float: left;
        position: relative;
        width: 30px;
        height: 30px;
        top: -60px;
        margin-right: 2px;
        font-size: 30px;
        text-decoration: none
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner .social-share-links .share-link span {
        position: absolute;
        left: 8px;
        top: 8px;
        font-size: 14px;
        color: #fff
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner .social-share-links .share-link.facebook {
        color: #496eb5;
        transition: top .3s
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner .social-share-links .share-link.twitter {
        color: #69c8ed;
        transition: top .3s .1s
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner .social-share-links .share-link.pinterest {
        color: #ef4646;
        transition: top .3s .2s
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner .social-share-links .share-link:hover {
        width: 34px;
        height: 34px;
        margin: -2px 0 0 -2px;
        font-size: 34px
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner .social-share-links .share-link:hover span {
        font-size: 18px
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner .navigation-button {
        width: 50%;
        height: 100%;
        top: 0;
        margin: 0;
        z-index: 2
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner .navigation-button .icon-container {
        position: absolute;
        width: 84px;
        height: 64px;
        top: 50%;
        margin-top: -32px;
        font-size: 64px;
        text-align: center;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=40)";
        filter: alpha(opacity=40);
        -moz-opacity: .4;
        -khtml-opacity: .4;
        opacity: .4;
        zoom:1}
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner .navigation-button:hover .icon-container {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=60)";
        filter: alpha(opacity=60);
        -moz-opacity: .6;
        -khtml-opacity: .6;
        opacity: .6;
        zoom:1}
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner .navigation-button.prev {
        left: 0
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner .navigation-button.prev .icon-container {
        left: -84px;
        border-radius: 0 5px 5px 0;
        transition: left .3s
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner .navigation-button.next {
        right: 0
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner .navigation-button.next .icon-container {
        right: -84px;
        border-radius: 5px 0 0 5px;
        transition: right .3s
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner .item-link {
        position: absolute;
        display: block;
        bottom: 20px;
        right: 20px;
        padding: 4px 10px 4px 30px;
        font-size: 13px;
        font-weight: 700;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=90)";
        filter: alpha(opacity=90);
        -moz-opacity: .9;
        -khtml-opacity: .9;
        opacity: .9;
        zoom:1;font-family: 'PT Sans',sans-serif;
        text-decoration: none;
        border-radius: 4px;
        z-index: 3
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner .item-link.no-link,.popup-overlay.popup-4.no-thumbs .footer,.popup-overlay.popup-4.single-item-popup .footer {
        display: none
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner .item-link:hover {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
        filter: alpha(opacity=100);
        -moz-opacity: 1;
        -khtml-opacity: 1;
        opacity: 1;
        zoom:1}
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner .item-link span {
        position: absolute;
        left: 8px;
        top: 4px;
        font-size: 17px
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner:hover .social-share-links .share-link {
        top: 0
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner:hover .social-share-links .share-link.facebook {
        transition: top .3s .2s
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner:hover .social-share-links .share-link.twitter {
        transition: top .3s .1s
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner:hover .social-share-links .share-link.pinterest {
        transition: top .3s
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner:hover .navigation-button.prev .icon-container {
        left: 0;
        transition: left .3s
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner:hover .navigation-button.next .icon-container {
        right: 0;
        transition: right .3s
    }
    
    .popup-overlay.popup-4 .slideshow-container .slideshow-container-inner:hover .carousel-container .carousel-item .image-text .description-wrapper {
        max-height: 62px
    }
    
    .popup-overlay.popup-4 .footer {
        width: 120px;
        height: auto;
        left: auto;
        right: 20px;
        top: 40px;
        bottom: 20px;
        padding-left: 35px;
        overflow: hidden
    }
    
    .popup-overlay.popup-4 .footer .thumbs-container {
        height: 100%;
        margin: 0
    }
    
    .popup-overlay.popup-4 .footer .thumbs-container .slideshow-thumbs-container {
        height: 100%;
        overflow: visible
    }
    
    .popup-overlay.popup-4 .footer .thumbs-container .slideshow-thumbs-container .thumbs {
        height: auto;
        white-space: normal
    }
    
    .popup-overlay.popup-4 .footer .thumbs-container .thumb {
        position: relative
    }
    
    .popup-overlay.popup-4 .footer .thumbs-container .thumb .image-thumb {
        width: 120px;
        height: 76px;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
        filter: alpha(opacity=100);
        -moz-opacity: 1;
        -khtml-opacity: 1;
        opacity: 1;
        zoom:1;margin: 0 0 15px
    }
    
    .popup-overlay.popup-4 .footer .thumbs-container .thumb .image-thumb:hover img {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=90)";
        filter: alpha(opacity=90);
        -moz-opacity: .9;
        -khtml-opacity: .9;
        opacity: .9;
        zoom:1}
    
    .popup-overlay.popup-4 .footer .thumbs-container .thumb:first-child .image-thumb {
        margin-left: auto
    }
    
    .popup-overlay.popup-4 .footer .thumbs-container .thumb:last-child .image-thumb {
        margin: 0
    }
    
    .popup-overlay.popup-4 .footer .thumbs-container .thumb.current .image-thumb {
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
        filter: alpha(opacity=100);
        -moz-opacity: 1;
        -khtml-opacity: 1;
        opacity: 1;
        zoom:1}
    
    .popup-overlay.popup-4 .footer .thumbs-container .thumb.current:before {
        position: absolute;
        content: '';
        width: 0;
        height: 0;
        left: -36px;
        top: 28px;
        border: 10px solid;
        border-color: transparent #000 transparent transparent;
        -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=30)";
        -moz-opacity: .3;
        -khtml-opacity: .3;
        opacity: .3;
        zoom:1;-webkit-filter: blur(2px);
        filter: blur(2px);
        z-index: 20
    }
    
    .popup-overlay.popup-4 .footer .thumbs-container .thumb.current:after {
        position: absolute;
        content: '';
        width: 0;
        height: 0;
        left: -35px;
        top: 28px;
        border: 10px solid transparent;
        z-index: 21
    }
    
    .popup-overlay.popup-4 .footer .shadow-hide {
        position: absolute;
        width: 15px;
        height: 100%;
        left: 20px;
        top: 0;
        z-index: 22
    }
    
    .popup-overlay.popup-4.no-thumbs .slideshow-container,.popup-overlay.popup-4.single-item-popup .slideshow-container {
        padding-right: 20px
    }
    
    .popup-overlay.popup-4.show-share-buttons .slideshow-container-inner .social-share-links.has-share-link {
        display: block
    }
    
    .popup-overlay.popup-4.no-description .slideshow-container .carousel-container .carousel-item .image-text .description-wrapper,.popup-overlay.popup-4.no-description .slideshow-container .carousel-container .carousel-item .no-title .image-text,.popup-overlay.popup-4.no-title .slideshow-container .carousel-container .carousel-item .image-text .title,.popup-overlay.popup-4.no-title .slideshow-container .carousel-container .carousel-item .no-description .image-text,.popup-overlay.popup-4.no-title.no-description .carousel-item .image-text,.popup-overlay.popup-4.video-popup .slideshow-container .slideshow-container-inner .social-share-links {
        display: none
    }
    
    .popup-overlay.popup-4.no-title .slideshow-container .carousel-container .carousel-item .image-text .description {
        margin-top: 16px
    }
    
    .popup-overlay.popup-4.video-popup .slideshow-container .slideshow-container-inner .navigation-button {
        width: 84px;
        height: 64px;
        top: 50%;
        margin-top: -32px
    }
    
    .popup-overlay.popup-4.video-popup .slideshow-container .slideshow-container-inner .navigation-button .icon-container {
        top: 0;
        margin-top: 0
    }
    
    .popup-overlay.popup-4.tablet-mode .slideshow-container .slideshow-container-inner .social-share-links .share-link {
        top: 0
    }
    
    .popup-overlay.popup-4.tablet-mode .slideshow-container .slideshow-container-inner .navigation-button.prev .icon-container {
        left: 0
    }
    
    .popup-overlay.popup-4.tablet-mode .slideshow-container .slideshow-container-inner .navigation-button.next .icon-container {
        right: 0
    }
    
    .popup-overlay.popup-4.tablet-mode .slideshow-container .slideshow-container-inner .carousel-container .carousel-item .image-text .description-wrapper {
        max-height: 62px
    }
    
    .skin-instance-controller {
        position: relative;
        margin: 0;
        height: 100%
    }
    
    .password-body .progress {
        position: relative;
        height: 4px;
        display: block;
        width: 100%;
        background-color: #0288D1;
        border-radius: 2px;
        background-clip: padding-box;
        margin: .5rem 0 1rem;
        overflow: hidden;
        opacity: 0
    }
    
    .password-body.no-margin {
        margin: 0
    }
    
    .password-body .progress .indeterminate {
        background-color: #d3efff
    }
    
    .password-body .progress .indeterminate:after,.password-body .progress .indeterminate:before {
        content: '';
        position: absolute;
        background-color: inherit;
        left: 0;
        will-change: left,right;
        top: 0;
        bottom: 0
    }
    
    .password-body .progress .indeterminate:before {
        -webkit-animation: indeterminate 2.1s cubic-bezier(.65,.815,.735,.395) infinite;
        animation: indeterminate 2.1s cubic-bezier(.65,.815,.735,.395) infinite
    }
    
    .password-body .progress .indeterminate:after {
        -webkit-animation: indeterminate-short 2.1s cubic-bezier(.165,.84,.44,1) infinite;
        animation: indeterminate-short 2.1s cubic-bezier(.165,.84,.44,1) infinite;
        -webkit-animation-delay: 1.15s;
        animation-delay: 1.15s
    }
    
    @-webkit-keyframes indeterminate {
        0% {
            left: -35%;
            right: 100%
        }
    
        100%,60% {
            left: 100%;
            right: -90%
        }
    }
    
    @keyframes indeterminate {
        0% {
            left: -35%;
            right: 100%
        }
    
        100%,60% {
            left: 100%;
            right: -90%
        }
    }
    
    @-webkit-keyframes indeterminate-short {
        0% {
            left: -200%;
            right: 100%
        }
    
        100%,60% {
            left: 107%;
            right: -8%
        }
    }
    
    @keyframes indeterminate-short {
        0% {
            left: -200%;
            right: 100%
        }
    
        100%,60% {
            left: 107%;
            right: -8%
        }
    }
    
    .password-main {
        position: fixed;
        top: 0;
        bottom: 0;
        height: 100%;
        width: 100%;
        background-color: #F5F5F5;
        -webkit-transition-property: opacity,-webkit-transform;
        -o-transition-property: opacity,-o-transform;
        transition-property: opacity,transform;
        transition-property: opacity,transform,-webkit-transform,-o-transform;
        -webkit-transition-timing-function: cubic-bezier(.4,0,1,1);
        -o-transition-timing-function: cubic-bezier(.4,0,1,1);
        transition-timing-function: cubic-bezier(.4,0,1,1);
        -webkit-transition-duration: 225ms;
        -o-transition-duration: 225ms;
        transition-duration: 225ms
    }
    
    .password-main .password-back-button {
        color: #0288D1;
        font-size: 20px;
        margin: 15px
    }
    
    .password-main .password-body {
        position: absolute;
        width: 330px;
        height: 330px;
        left: 0;
        right: 0;
        top: 0;
        bottom: 0;
        margin: auto
    }
    
    .password-main .password-body .password-input,.password-main .password-body .password-input-field,.password-main .password-body .password-label {
        width: 330px;
        color: rgba(0,0,0,.26)
    }
    
    .password-main .password-body .password-input-field {
        font-size: 16px;
        height: 20px;
        border: none;
        background: 0 0;
        color: rgba(0,0,0,.26);
        border-top: 1px solid transparent;
        border-bottom: 1px solid rgba(0,0,0,.26)
    }
    
    .password-main .password-body .password-input-field.state-focused {
        border-top: 0 solid transparent;
        border-bottom: 2px solid #0288D1;
        color: #000
    }
    
    .password-main .password-body .password-input-field.state-error {
        border-bottom: 2px solid #BC2113
    }
    
    .password-main .password-body .password-label {
        margin-bottom: 5px
    }
    
    .password-main .password-body .password-label.label-focused:not(.state-error) {
        color: #0288D1
    }
    
    .password-main .password-body .password-input {
        margin-bottom: 10px
    }
    
    .password-main .password-error {
        color: #BC2113;
        margin-bottom: 15px
    }
    
    .password-main.preview .password-body {
        margin: 20% auto auto
    }
    
    .password-button {
        width: 300px;
        background-image: none;
        border: 0;
        -webkit-box-shadow: 0 2px 2px 0 rgba(0,0,0,.14),0 1px 5px 0 rgba(0,0,0,.12),0 3px 1px -2px rgba(0,0,0,.2);
        box-shadow: 0 2px 2px 0 rgba(0,0,0,.14),0 1px 5px 0 rgba(0,0,0,.12),0 3px 1px -2px rgba(0,0,0,.2);
        cursor: pointer;
        display: inline-block;
        font-size: 14px!important;
        font-weight: 500;
        line-height: 1;
        margin: 0;
        max-width: 100%;
        min-width: 5.5rem;
        padding: .6875rem 1rem;
        position: relative;
        text-align: center;
        text-transform: uppercase;
        -moz-user-select: none;
        user-select: none;
        vertical-align: middle;
        white-space: nowrap;
        z-index: 20;
        border-radius: 2px!important;
        -webkit-transition-duration: .3s;
        -o-transition-duration: .3s;
        transition-duration: .3s;
        -webkit-transition-property: background-color,color,-webkit-box-shadow;
        -o-transition-property: background-color,box-shadow,color;
        transition-property: background-color,box-shadow,color;
        transition-property: background-color,box-shadow,color,-webkit-box-shadow;
        -webkit-transition-timing-function: cubic-bezier(.4,0,.2,1);
        -o-transition-timing-function: cubic-bezier(.4,0,.2,1);
        transition-timing-function: cubic-bezier(.4,0,.2,1)
    }
    
    .drop-panel-wrapper .slide-navigation-panel .footer,.drop-panel-wrapper .slide-navigation-panel .header,body #privacy-policy-bar {
        display: none
    }
    
    .password-button.variation-action {
        color: #fff;
        background: #0288D1
    }
    
    .password-button.state-disabled {
        background-color: rgba(0,0,0,.12)!important;
        color: rgba(0,0,0,.26)!important;
        cursor: not-allowed!important
    }
    
    @media only screen and (max-width: 414px) {
        .password-body {
            position:initial!important;
            width: 90%!important
        }
    
        .password-body .password-input,.password-body .password-input-field {
            width: 100%!important
        }
    
        .password-body .password-button {
            padding: .6875rem 0!important;
            width: 100%!important
        }
    }
    
    body.view-mode #privacy-policy-bar {
        line-height: 32px;
        font: 15px;
        background-color: #000;
        color: #fff;
        text-align: center;
        display: block
    }
    
    body .privacy-policy-dialog {
        padding: 15px;
        background-color: #fff;
        border: 1px solid #000
    }
    
    body .privacy-policy-dialog .privacy-policy-dialog-content {
        overflow: auto;
        white-space: normal;
        margin-bottom: 15px
    }
    
    body .privacy-policy-dialog .privacy-policy-dialog-footer {
        text-align: center;
        border-top: 1px solid #ccc;
        padding-top: 15px
    }
    
    body .privacy-policy-dialog .privacy-policy-dialog-title {
        list-style: outside;
        font-size: 30px;
        text-align: center;
        font-weight: 700;
        margin-bottom: 15px;
        border-bottom: 1px solid #ccc;
        padding-bottom: 15px
    }
    
    body .privacy-policy-dialog .dialog-text {
        font-size: 14px;
        text-align: left
    }
    
    body .privacy-policy-dialog .privacy-policy-dialog-button {
        padding: 0 15px
    }
    
    .message-dialog-panel {
        width: 100%;
        height: 100%;
        top: 0;
        position: fixed;
        z-index: 9999999999;
        background-color: rgba(22,22,22,.5)
    }
    
    .message-dialog-panel .message-dialog-container {
        position: relative;
        margin: 0 auto;
        top: 33%;
        width: 320px;
        background-color: #fff;
        border-radius: 4px;
        text-align: center
    }
    
    .message-dialog-panel .message-dialog-title {
        font-size: 18px;
        padding: 10px;
        border-bottom: 1px solid #f8f8ff
    }
    
    .message-dialog-panel .message-dialog-content {
        font-size: 15px;
        padding: 15px 5px;
        min-height: 33px
    }
    
    .message-dialog-panel .message-dialog-close {
        padding: 5px;
        margin: 10px;
        font-size: 15px;
        cursor: pointer
    }
    
    body.mobile-desktop-mode .slide-navigation-panel .close-icon-content {
        right: 14px;
        top: 14px;
        font-size: 20px
    }
    
    .drop-panel-wrapper .slide-navigation-panel .scrolling-pane,.drop-panel-wrapper .slide-navigation-panel .scrolling-view {
        position: relative
    }
    
    .drop-panel-wrapper .slide-navigation-panel .scrolling-view {
        top: 0
    }
    
    .slide-navigation-panel {
        position: relative;
        text-align: left;
        background-color: transparent;
        display: inline-block;
        height: 100%
    }
    
    .slide-navigation-panel.vertical {
        display: block;
        height: auto
    }
    
    .slide-navigation-panel .close-icon-content {
        position: absolute;
        right: 12px;
        top: 12px;
        font-size: 14px;
        cursor: pointer
    }
    
    .slide-navigation-panel .header {
        height: 40px
    }
    
    .slide-navigation-panel .footer {
        position: absolute;
        right: 0;
        left: 0;
        bottom: 0
    }
    
    .slide-navigation-panel .scrolling-pane,.slide-navigation-panel .scrolling-view {
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0
    }
    
    .slide-navigation-panel .scrolling-view {
        top: 40px
    }
    
    .slide-navigation-panel .page-content {
        position: relative
    }
    
    .slide-navigation-panel .title-container {
        padding-right: 20px;
        cursor: pointer
    }
    
    .slide-navigation-panel .page-item {
        border-bottom: 1px solid rgba(255,255,255,.2)
    }
    
    .slide-navigation-panel .icon-container {
        position: absolute;
        top: 0;
        bottom: 0;
        right: 100%;
        width: 45px;
        text-align: center
    }
    
    .slide-navigation-panel .hierarchy-icon {
        display: none;
        max-width: 45px;
        cursor: pointer;
        font-size: 120%
    }
    
    .slide-navigation-panel .hierarchy-has-children>.hierarchy-item-content>.hierarchy-item-container .open-icon {
        display: inline-block
    }
    
    .slide-navigation-panel .hierarchy-has-children.open>.hierarchy-item-content>.hierarchy-item-container .open-icon {
        display: none
    }
    
    .slide-navigation-panel .hierarchy-has-children.open>.hierarchy-item-content>.hierarchy-item-container .close-icon {
        display: inline-block
    }
    
    .slide-navigation-panel .hierarchy-has-children.open>.hierarchy-item-content>.hierarchy-children-container {
        display: block
    }
    
    .slide-navigation-panel .hierarchy-has-children>.hierarchy-item-content>.hierarchy-children-container {
        display: none
    }
    
    .slide-navigation-panel a {
        color: inherit
    }
    
    .slide-navigation-panel .hierarchy-level-0>.hierarchy-item-content>.hierarchy-item-container .page-item {
        padding-left: 45px
    }
    
    .slide-navigation-panel .hierarchy-level-1 .title-container {
        font-size: 80%
    }
    
    .slide-navigation-panel .hierarchy-level-1>.hierarchy-item-content>.hierarchy-item-container .page-item {
        padding-left: 60px
    }
    
    .slide-navigation-panel .hierarchy-level-2>.hierarchy-item-content>.hierarchy-item-container .page-item {
        padding-left: 75px
    }
    
    .slide-navigation-panel .hierarchy-level-3>.hierarchy-item-content>.hierarchy-item-container .page-item {
        padding-left: 90px
    }
    
    #freemium-footer-iframe {
        border: none;
        overflow-y: hidden;
        overflow-x: hidden;
        display: block;
        position: fixed;
        left: 0;
        bottom: 0;
        width: 100%
    }
    
    body.design-mode #freemium-footer {
        display: none
    }
    
    .image-sprite-header-footer-sections-add {
        display: inline-block;
        background: url(viewer-sprite.png) top left no-repeat;
        background-position: 0 -32px!important;
        width: 12px;
        height: 12px
    }
    
    .image-sprite-video-play-button-hover {
        display: inline-block;
        background: url(viewer-sprite.png) top left no-repeat;
        background-position: 0 0!important;
        width: 42px;
        height: 29px
    }
    
    .image-sprite-video-play-button {
        display: inline-block;
        background: url(viewer-sprite.png) top left no-repeat;
        background-position: -45px 0!important;
        width: 42px;
        height: 29px
    }
    </style>
</head>
<body>
    
</body>
</html>
<body class="user-interaction-normal hover-supported scrolling-mode-normal preview-mode site-viewer pc pc-client view-mode full-screen-view pc-desktop-mode">
    <div id="fontdetectHelper" style="position: absolute; visibility: hidden; top: -200px; left: -100000px; width: 100000px; height: 200px; font-size: 100px;">
        <span style="font-family: &quot;lato light&quot;, fantasy;">abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ</span>
    </div>
    <div class="body-element-container"><div class="body-element-wrapper"><div id="body-element" class="view-mode"><div id="offset-anchor"></div><div class="design-element page-element" id="id1626439686754" data-element-id="id1626439686754"><div class="element-main-box positioned" data-element-id="id1626439686754"><div class="element-background-layer positioned absolute-fill element-border-target design-element-border-target fixed-attachment-background fixed-page-background" data-element-id="id1626439686754" style="background-color: rgb(214, 218, 222);"></div><div class="element-background-image state-displayed fixed-attachment-background fixed-page-background image-box-new optimize-speed state-no-image"><div class="image-box-image-wrapper horizontal-center vertical-center stretchedToFill non-tile-layout" style="width: 1304px; height: 658px;"><div class="image-box-background-image"></div></div></div><div class="page-element-border-box element-border-target positioned design-element-border-box" data-element-id="id1626439686754"><div class="header-section page-section positioned" data-element-id="id1626439686754"></div><div class="element-content-box element-padding-box positioned" data-element-id="id1626439686754"><div class="page-element-size-box element-size-box positioned element-size-target" data-element-id="id1626439686754" style="min-height: 0px;"><div class="master-page-mobile-content-container" data-element-id="id1626439686754"></div><div class="page-content-container content-container-type" data-element-id="id1626439686754"><div class="page-element element-content"><div class="design-element positioned page-content-element block-element is-page-child" id="id1402310978797" data-element-id="1402310978797" style="margin: 0px;"><div class="element-main-box positioned page-content-element" data-element-id="1402310978797"><div class="element-background-layer element-border-target design-element-border-target page-content-element" data-element-id="1402310978797" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target positioned design-element-border-box page-content-element" data-element-id="1402310978797" style="border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box element-padding-box positioned page-content-element" data-element-id="1402310978797" style="padding: 0px;"><div class="page-content-element-size-box element-size-box positioned element-size-target page-content-element" data-element-id="1402310978797" style="min-height: 0px;"><div class="page-content-content-container content-container-type positioned page-content-element" data-element-id="1402310978797"><div class="base-page-content-element"> <div class="main-sections-container border-box-sizing"><div class="sections-wrapper"><div class="positioned"><div class="design-element element-size-box page-section-element section-element hidden-design-element is-page-child" id="idmasterPageContentSectionId" data-element-id="masterPageContentSectionId"><section class="html-element page-section-element" data-element-id="masterPageContentSectionId"><div class="element-main-box design-element-main-box page-section-element state-hidden" data-element-id="masterPageContentSectionId"><div class="element-background-layer element-border-target design-element-background-layer page-section-element" data-element-id="masterPageContentSectionId" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box page-section-element" data-element-id="masterPageContentSectionId" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box page-section-element" data-element-id="masterPageContentSectionId"><div class="content-container content-container-type element-size-box element-size-target page-section-element section-element-size-box" data-element-id="masterPageContentSectionId"></div></div></div></div></section></div><div class="design-element element-size-box page-section-element is-page-child section-element first-section first-main-section" id="id1632914223274" data-element-id="id1632914223274"><section class="html-element page-section-element" data-element-id="id1632914223274"><div class="element-main-box design-element-main-box page-section-element" data-element-id="id1632914223274"><div class="element-background-layer element-border-target design-element-background-layer page-section-element" data-element-id="id1632914223274" style="background-color: rgb(251, 253, 255);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box page-section-element" data-element-id="id1632914223274" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box page-section-element" data-element-id="id1632914223274"><div class="content-container content-container-type element-size-box element-size-target page-section-element section-element-size-box" data-element-id="id1632914223274" style="min-height: 1444px;"><div class="design-element element-size-box user-selectable-element clickable-element has-popup image-element is-section-child block-element" id="id1632914223275" data-element-id="id1632914223275" style="left: 0px; right: 0px; top: 0px; z-index: 8;"><div class="element-main-box design-element-main-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1632914223275" style="z-index: 8;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element has-popup image-element" data-element-id="id1632914223275" style="background-color: rgb(107, 206, 224);"></div><div class="element-background-image design-element-background-image state-displayed image-box-new optimize-speed state-image-loaded"><div class="image-box-image-wrapper horizontal-center vertical-center stretchedToFill non-tile-layout use-image-element" style="width: 1304px; height: 600px;"><div class="image-box-background-image" style="background-image: url(&quot;https://images.unsplash.com/photo-1432888498266-38ffec3eaf0a?ixlib=rb-1.2.1&amp;q=85&amp;fm=jpg&amp;crop=entropy&amp;cs=srgb&amp;w=1450&quot;);"></div><img class="image-box-image-new" src="https://images.unsplash.com/photo-1432888498266-38ffec3eaf0a?ixlib=rb-1.2.1&amp;q=85&amp;fm=jpg&amp;crop=entropy&amp;cs=srgb&amp;w=1450" width="1304" height="867" style="width: 1304px; height: 867px; margin-top: -133px; margin-left: 0px;"></div></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1632914223275" style="border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1632914223275"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element has-popup image-element" data-element-id="id1632914223275" style="min-height: 600px;"></div></div></div></div></div><div class="design-element element-size-box has-rich-content user-selectable-element clickable-element has-rich-content has-text is-section-child" id="id1632914223276" data-element-id="id1632914223276" style="left: 50%; top: 949px; margin-left: -459px; z-index: 9;"><div class="element-main-box design-element-main-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223276" style="z-index: 9;"><div class="element-background-layer element-border-target design-element-background-layer has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223276" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223276" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223276"><div class="content-container content-container-type element-size-box element-size-target has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223276" style="width: 239px; min-height: 39px;"><div class="rich-text-element-content absolute-fill element-content dir-ltr" style="background: none; text-align: center; color: rgb(51, 51, 51); line-height: 1.2; letter-spacing: 0px; font-size: 25px; font-family: &quot;Lato Light&quot;;"><div class="rich-text-positioning-wrapper vertical-alignment-top"><div class="rich-text-content common-rich-content-style has-content"><div><strong><span class="theme-text-color-3-4">Calendário Escolar</span></strong></div></div></div></div></div></div></div></div></div><div class="design-element element-size-box has-rich-content user-selectable-element clickable-element has-rich-content has-text is-section-child" id="id1632914223277" data-element-id="id1632914223277" style="left: 50%; top: 988px; margin-left: -450px; z-index: 10;"><div class="element-main-box design-element-main-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223277" style="z-index: 10;"><div class="element-background-layer element-border-target design-element-background-layer has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223277" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223277" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223277"><div class="content-container content-container-type element-size-box element-size-target has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223277" style="width: 239px; min-height: 63px;"><div class="rich-text-element-content absolute-fill element-content dir-ltr" style="background: none; text-align: center; color: rgb(51, 51, 51); line-height: 1.2; letter-spacing: 0px; font-size: 15px; font-family: &quot;Lato Light&quot;;"><div class="rich-text-positioning-wrapper vertical-alignment-top"><div class="rich-text-content common-rich-content-style has-content"><div data-line-height="1.4"><span class="theme-text-color-2-2"><span style="font-size:16px;">Para&nbsp;consultar&nbsp;o Calendário Escolar com toda a programação&nbsp;<br>do ano letivo.</span></span><br><span style="font-size:16px;"></span></div></div></div></div></div></div></div></div></div><div class="design-element element-size-box has-rich-content user-selectable-element clickable-element has-rich-content has-text is-section-child" id="id1632914223279" data-element-id="id1632914223279" style="left: 50%; top: 949px; margin-left: 196px; z-index: 11;"><div class="element-main-box design-element-main-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223279" style="z-index: 11;"><div class="element-background-layer element-border-target design-element-background-layer has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223279" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223279" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223279"><div class="content-container content-container-type element-size-box element-size-target has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223279" style="width: 268px; min-height: 39px;"><div class="rich-text-element-content absolute-fill element-content dir-ltr" style="background: none; text-align: center; color: rgb(51, 51, 51); line-height: 1.2; letter-spacing: 0px; font-size: 25px; font-family: &quot;Lato Light&quot;;"><div class="rich-text-positioning-wrapper vertical-alignment-top"><div class="rich-text-content common-rich-content-style has-content"><div><strong><span class="theme-text-color-3-4">Calendário de Avaliações</span></strong></div></div></div></div></div></div></div></div></div><div class="design-element element-size-box has-rich-content user-selectable-element clickable-element has-rich-content has-text is-section-child" id="id1632914223280" data-element-id="id1632914223280" style="left: 50%; top: 988px; margin-left: 212px; z-index: 12;"><div class="element-main-box design-element-main-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223280" style="z-index: 12;"><div class="element-background-layer element-border-target design-element-background-layer has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223280" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223280" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223280"><div class="content-container content-container-type element-size-box element-size-target has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223280" style="width: 239px; min-height: 63px;"><div class="rich-text-element-content absolute-fill element-content dir-ltr" style="background: none; text-align: center; color: rgb(51, 51, 51); line-height: 1.2; letter-spacing: 0px; font-size: 15px; font-family: &quot;Lato Light&quot;;"><div class="rich-text-positioning-wrapper vertical-alignment-top"><div class="rich-text-content common-rich-content-style has-content"><div data-line-height="1.4"><span style="font-size:16px;"><span class="theme-text-color-2-2">Para&nbsp;consultar todas </span></span><span style="font-size:16px;"><span class="theme-text-color-2-2">as avaliações que serão&nbsp;</span></span><span style="font-size:16px;"><span class="theme-text-color-2-2">realizadas </span></span><br></div><div data-line-height="1.4"><span style="font-size:16px;"><span class="theme-text-color-2-2">durante o ano letivo.</span></span><br></div></div></div></div></div></div></div></div></div><div class="design-element element-size-box has-rich-content user-selectable-element clickable-element has-rich-content has-text is-section-child" id="id1632914223281" data-element-id="id1632914223281" style="left: 50%; top: 949px; margin-left: -119px; z-index: 13;"><div class="element-main-box design-element-main-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223281" style="z-index: 13;"><div class="element-background-layer element-border-target design-element-background-layer has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223281" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223281" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223281"><div class="content-container content-container-type element-size-box element-size-target has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223281" style="width: 239px; min-height: 39px;"><div class="rich-text-element-content absolute-fill element-content dir-ltr" style="background: none; text-align: center; color: rgb(51, 51, 51); line-height: 1.2; letter-spacing: 0px; font-size: 25px; font-family: &quot;Lato Light&quot;;"><div class="rich-text-positioning-wrapper vertical-alignment-top"><div class="rich-text-content common-rich-content-style has-content"><div><span class="theme-text-color-3-4"><strong>Quadro de Horários</strong></span></div></div></div></div></div></div></div></div></div><div class="design-element element-size-box has-rich-content user-selectable-element clickable-element has-rich-content has-text is-section-child" id="id1632914223282" data-element-id="id1632914223282" style="left: 50%; top: 988px; margin-left: -119px; z-index: 14;"><div class="element-main-box design-element-main-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223282" style="z-index: 14;"><div class="element-background-layer element-border-target design-element-background-layer has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223282" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223282" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223282"><div class="content-container content-container-type element-size-box element-size-target has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1632914223282" style="width: 239px; min-height: 63px;"><div class="rich-text-element-content absolute-fill element-content dir-ltr" style="background: none; text-align: center; color: rgb(51, 51, 51); line-height: 1.2; letter-spacing: 0px; font-size: 15px; font-family: &quot;Lato Light&quot;;"><div class="rich-text-positioning-wrapper vertical-alignment-top"><div class="rich-text-content common-rich-content-style has-content"><div data-line-height="1.4"><span class="theme-text-color-2-2"><span style="font-size:16px;">Para&nbsp;consultar&nbsp;o Quadro de&nbsp;Horários&nbsp;com os&nbsp;</span></span><br></div><div data-line-height="1.4"><span class="theme-text-color-2-2"><span style="font-size:16px;">horários&nbsp;das turmas.</span></span></div></div></div></div></div></div></div></div></div><div class="design-element element-size-box has-rich-content user-selectable-element clickable-element has-rich-content has-text is-section-child" id="id1649331152590" data-element-id="id1649331152590" style="left: 50%; top: 1280px; margin-left: -119px; z-index: 15;"><div class="element-main-box design-element-main-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1649331152590" style="z-index: 15;"><div class="element-background-layer element-border-target design-element-background-layer has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1649331152590" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1649331152590" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1649331152590"><div class="content-container content-container-type element-size-box element-size-target has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1649331152590" style="width: 239px; min-height: 39px;"><div class="rich-text-element-content absolute-fill element-content dir-ltr" style="background: none; text-align: center; color: rgb(51, 51, 51); line-height: 1.2; letter-spacing: 0px; font-size: 25px; font-family: &quot;Lato Light&quot;;"><div class="rich-text-positioning-wrapper vertical-alignment-top"><div class="rich-text-content common-rich-content-style has-content"><div><strong><span class="theme-text-color-3-4">Eventos Escolares</span></strong></div></div></div></div></div></div></div></div></div><div class="design-element element-size-box has-rich-content user-selectable-element clickable-element has-rich-content has-text is-section-child" id="id1649331152591" data-element-id="id1649331152591" style="left: 50%; top: 1319px; margin-left: -110px; z-index: 16;"><div class="element-main-box design-element-main-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1649331152591" style="z-index: 16;"><div class="element-background-layer element-border-target design-element-background-layer has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1649331152591" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1649331152591" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1649331152591"><div class="content-container content-container-type element-size-box element-size-target has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1649331152591" style="width: 230px; min-height: 42px;"><div class="rich-text-element-content absolute-fill element-content dir-ltr" style="background: none; text-align: center; color: rgb(51, 51, 51); line-height: 1.2; letter-spacing: 0px; font-size: 15px; font-family: &quot;Lato Light&quot;;"><div class="rich-text-positioning-wrapper vertical-alignment-top"><div class="rich-text-content common-rich-content-style has-content"><div data-line-height="1.4"><span class="theme-text-color-2-2"><span style="font-size:16px;">Fique por dentro de todos os eventos escolares.</span></span><br></div></div></div></div></div></div></div></div></div><div class="design-element group-element user-selectable-element clickable-element is-section-child forwardLayerEvents" id="id1656603720948" data-element-id="id1656603720948" style="left: 50%; top: 631px; margin-left: -20px; z-index: 17;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element" data-element-id="id1656603720948" style="z-index: 17;"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element" data-element-id="id1656603720948" style="width: 40px; min-height: 8px;"><div class="design-element element-size-box user-selectable-element clickable-element catchLayerEvents is-section-child" id="id1656603720949" data-element-id="id1656603720949" style="left: 0px; top: 0px; z-index: 1;"><div class="element-main-box design-element-main-box user-selectable-element clickable-element" data-element-id="id1656603720949" style="z-index: 1;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element" data-element-id="id1656603720949" style="background-color: rgb(0, 48, 97);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element" data-element-id="id1656603720949" style="border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element" data-element-id="id1656603720949"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element" data-element-id="id1656603720949" style="width: 8px; min-height: 8px;"></div></div></div></div></div><div class="design-element element-size-box user-selectable-element clickable-element catchLayerEvents is-section-child" id="id1656603720950" data-element-id="id1656603720950" style="left: 16px; top: 0px; z-index: 2;"><div class="element-main-box design-element-main-box user-selectable-element clickable-element" data-element-id="id1656603720950" style="z-index: 2;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element" data-element-id="id1656603720950" style="background-color: rgb(0, 48, 97);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element" data-element-id="id1656603720950" style="border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element" data-element-id="id1656603720950"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element" data-element-id="id1656603720950" style="width: 8px; min-height: 8px;"></div></div></div></div></div><div class="design-element element-size-box user-selectable-element clickable-element catchLayerEvents is-section-child" id="id1656603720951" data-element-id="id1656603720951" style="left: 32px; top: 0px; z-index: 3;"><div class="element-main-box design-element-main-box user-selectable-element clickable-element" data-element-id="id1656603720951" style="z-index: 3;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element" data-element-id="id1656603720951" style="background-color: rgb(0, 48, 97);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element" data-element-id="id1656603720951" style="border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element" data-element-id="id1656603720951"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element" data-element-id="id1656603720951" style="width: 8px; min-height: 8px;"></div></div></div></div></div></div></div></div><div class="design-element element-size-box has-rich-content user-selectable-element clickable-element has-rich-content has-text is-section-child" id="id1656603720952" data-element-id="id1656603720952" style="left: 50%; top: 659px; margin-left: -263.5px; z-index: 18;"><h2 class="html-element has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1656603720952"><div class="element-main-box design-element-main-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1656603720952" style="z-index: 18;"><div class="element-background-layer element-border-target design-element-background-layer has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1656603720952" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1656603720952" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1656603720952"><div class="content-container content-container-type element-size-box element-size-target has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1656603720952" style="width: 527px; min-height: 86px;"><div class="rich-text-element-content absolute-fill element-content dir-ltr" style="background: none; text-align: left; color: rgb(0, 0, 0); line-height: 1.2; letter-spacing: 0px; font-size: 72px; font-family: &quot;Lato Light&quot;;"><div class="rich-text-positioning-wrapper vertical-alignment-top"><div class="rich-text-content common-rich-content-style has-content"><div style="text-align: center;"><font color="#003061"><span style="font-size: 48px;">Vida <strong>Escolar</strong></span></font></div></div></div></div></div></div></div></div></h2></div><div class="design-element element-size-box has-rich-content user-selectable-element clickable-element has-rich-content has-text is-section-child" id="id1683218937649" data-element-id="id1683218937649" style="left: 50%; top: 1280px; margin-left: -459px; z-index: 19;"><div class="element-main-box design-element-main-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1683218937649" style="z-index: 19;"><div class="element-background-layer element-border-target design-element-background-layer has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1683218937649" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1683218937649" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1683218937649"><div class="content-container content-container-type element-size-box element-size-target has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1683218937649" style="width: 239px; min-height: 39px;"><div class="rich-text-element-content absolute-fill element-content dir-ltr" style="background: none; text-align: center; color: rgb(51, 51, 51); line-height: 1.2; letter-spacing: 0px; font-size: 25px; font-family: &quot;Lato Light&quot;;"><div class="rich-text-positioning-wrapper vertical-alignment-top"><div class="rich-text-content common-rich-content-style has-content"><div><span class="theme-text-color-3-4"><strong>Saída Pedagógica</strong></span></div></div></div></div></div></div></div></div></div><div class="design-element element-size-box has-rich-content user-selectable-element clickable-element has-rich-content has-text is-section-child" id="id1683218937650" data-element-id="id1683218937650" style="left: 50%; top: 1319px; margin-left: -459px; z-index: 20;"><div class="element-main-box design-element-main-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1683218937650" style="z-index: 20;"><div class="element-background-layer element-border-target design-element-background-layer has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1683218937650" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1683218937650" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1683218937650"><div class="content-container content-container-type element-size-box element-size-target has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1683218937650" style="width: 239px; min-height: 42px;"><div class="rich-text-element-content absolute-fill element-content dir-ltr" style="background: none; text-align: center; color: rgb(51, 51, 51); line-height: 1.2; letter-spacing: 0px; font-size: 15px; font-family: &quot;Lato Light&quot;;"><div class="rich-text-positioning-wrapper vertical-alignment-top"><div class="rich-text-content common-rich-content-style has-content"><div data-line-height="1.4"><span class="theme-text-color-2-2"><span style="font-size:16px;">Fique por dentro de todos as </span></span><br></div><div data-line-height="1.4"><span class="theme-text-color-2-2"><span style="font-size:16px;">saídas pedagógicas.</span></span><br></div></div></div></div></div></div></div></div></div><div class="design-element element-size-box has-rich-content user-selectable-element clickable-element has-rich-content has-text is-section-child" id="id1696418287164" data-element-id="id1696418287164" style="left: 50%; top: 1280px; margin-left: 212px; z-index: 21;"><div class="element-main-box design-element-main-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1696418287164" style="z-index: 21;"><div class="element-background-layer element-border-target design-element-background-layer has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1696418287164" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1696418287164" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1696418287164"><div class="content-container content-container-type element-size-box element-size-target has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1696418287164" style="width: 239px; min-height: 39px;"><div class="rich-text-element-content absolute-fill element-content dir-ltr" style="background: none; text-align: center; color: rgb(51, 51, 51); line-height: 1.2; letter-spacing: 0px; font-size: 25px; font-family: &quot;Lato Light&quot;;"><div class="rich-text-positioning-wrapper vertical-alignment-top"><div class="rich-text-content common-rich-content-style has-content"><div><span class="theme-text-color-3-4"><strong>Projetos Escolares</strong></span></div></div></div></div></div></div></div></div></div><div class="design-element element-size-box has-rich-content user-selectable-element clickable-element has-rich-content has-text is-section-child" id="id1696418287163" data-element-id="id1696418287163" style="left: 50%; top: 1319px; margin-left: 212px; z-index: 22;"><div class="element-main-box design-element-main-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1696418287163" style="z-index: 22;"><div class="element-background-layer element-border-target design-element-background-layer has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1696418287163" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1696418287163" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1696418287163"><div class="content-container content-container-type element-size-box element-size-target has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1696418287163" style="width: 239px; min-height: 42px;"><div class="rich-text-element-content absolute-fill element-content dir-ltr" style="background: none; text-align: center; color: rgb(51, 51, 51); line-height: 1.2; letter-spacing: 0px; font-size: 15px; font-family: &quot;Lato Light&quot;;"><div class="rich-text-positioning-wrapper vertical-alignment-top"><div class="rich-text-content common-rich-content-style has-content"><div data-line-height="1.4"><span class="theme-text-color-2-2"><span style="font-size:16px;">Fique por dentro de todos os projetos escolares.</span></span></div></div></div></div></div></div></div></div></div><div class="design-element element-size-box user-selectable-element clickable-element has-popup image-element is-section-child webzai-clickable-behaviour" id="id1719403332000" data-element-id="id1719403332000" style="left: 50%; top: 768px; margin-left: -431px; z-index: 23;"><a class="design-element-link-part no-decorations" target="_blank" href="https://docs.google.com/spreadsheets/d/1jNOq4SrRnTx3OAn-09sLDDN1HJymo4sxEwy_PcC6Kos/edit#gid=0"><div class="element-main-box design-element-main-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403332000" style="z-index: 23;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403332000" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-background-image design-element-background-image state-displayed image-box-new optimize-speed state-image-loaded"><div class="image-box-image-wrapper horizontal-center vertical-center stretchedToFill non-tile-layout use-image-element" style="width: 183px; height: 181px;"><div class="image-box-background-image" style="background-image: url(&quot;https://storage.googleapis.com/production-hostgator-brasil-v1-0-0/910/1831910/Ii0ZFo4Z/aac2fc06546e47b7815e8f770f2662a6&quot;);"></div><img class="image-box-image-new" src="https://storage.googleapis.com/production-hostgator-brasil-v1-0-0/910/1831910/Ii0ZFo4Z/aac2fc06546e47b7815e8f770f2662a6" width="183" height="183" style="width: 183px; height: 183px; margin-top: -1px; margin-left: 0px;"></div></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403332000" style="border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403332000"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403332000" style="width: 183px; min-height: 181px;"></div></div></div></div></a></div><div class="design-element element-size-box user-selectable-element clickable-element has-popup image-element is-section-child webzai-clickable-behaviour" id="id1719403386592" data-element-id="id1719403386592" style="left: 50%; top: 768px; margin-left: -90px; z-index: 24;"><a class="design-element-link-part no-decorations" target="_blank" href="https://drive.google.com/drive/folders/1R9fBdYUzpxyJTfs4d02PQNkMSRA16PuG?usp=sharing"><div class="element-main-box design-element-main-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403386592" style="z-index: 24;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403386592" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-background-image design-element-background-image state-displayed image-box-new optimize-speed state-image-loaded"><div class="image-box-image-wrapper horizontal-center vertical-center stretchedToFill non-tile-layout use-image-element" style="width: 183px; height: 181px;"><div class="image-box-background-image" style="background-image: url(&quot;https://storage.googleapis.com/production-hostgator-brasil-v1-0-0/910/1831910/Ii0ZFo4Z/7a945c77e96b42c2948525bf386ce0c5&quot;);"></div><img class="image-box-image-new" src="https://storage.googleapis.com/production-hostgator-brasil-v1-0-0/910/1831910/Ii0ZFo4Z/7a945c77e96b42c2948525bf386ce0c5" width="183" height="183" style="width: 183px; height: 183px; margin-top: -1px; margin-left: 0px;"></div></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403386592" style="border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403386592"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403386592" style="width: 183px; min-height: 181px;"></div></div></div></div></a></div><div class="design-element element-size-box user-selectable-element clickable-element has-popup image-element is-section-child webzai-clickable-behaviour" id="id1719403429692" data-element-id="id1719403429692" style="left: 50%; top: 768px; margin-left: 240px; z-index: 25;"><a class="design-element-link-part no-decorations" target="_blank" href="https://drive.google.com/drive/folders/1R9fBdYUzpxyJTfs4d02PQNkMSRA16PuG?usp=sharing"><div class="element-main-box design-element-main-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403429692" style="z-index: 25;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403429692" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-background-image design-element-background-image state-displayed image-box-new optimize-speed state-image-loaded"><div class="image-box-image-wrapper horizontal-center vertical-center stretchedToFill non-tile-layout use-image-element" style="width: 183px; height: 181px;"><div class="image-box-background-image" style="background-image: url(&quot;https://storage.googleapis.com/production-hostgator-brasil-v1-0-0/910/1831910/Ii0ZFo4Z/1ca7cce6d8394cb4b52c8825fcf82b92&quot;);"></div><img class="image-box-image-new" src="https://storage.googleapis.com/production-hostgator-brasil-v1-0-0/910/1831910/Ii0ZFo4Z/1ca7cce6d8394cb4b52c8825fcf82b92" width="183" height="183" style="width: 183px; height: 183px; margin-top: -1px; margin-left: 0px;"></div></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403429692" style="border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403429692"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403429692" style="width: 183px; min-height: 181px;"></div></div></div></div></a></div><div class="design-element element-size-box user-selectable-element clickable-element has-popup image-element is-section-child webzai-clickable-behaviour" id="id1719403514261" data-element-id="id1719403514261" style="left: 50%; top: 1105px; margin-left: -431px; z-index: 26;"><a class="design-element-link-part no-decorations" target="_blank" href="https://drive.google.com/drive/folders/1R9fBdYUzpxyJTfs4d02PQNkMSRA16PuG?usp=sharing"><div class="element-main-box design-element-main-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403514261" style="z-index: 26;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403514261" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-background-image design-element-background-image state-displayed image-box-new optimize-speed state-image-loaded"><div class="image-box-image-wrapper horizontal-center vertical-center stretchedToFill non-tile-layout use-image-element" style="width: 183px; height: 181px;"><div class="image-box-background-image" style="background-image: url(&quot;https://storage.googleapis.com/production-hostgator-brasil-v1-0-0/910/1831910/Ii0ZFo4Z/693fc155dd544bcb81e46a2c1c201f1b&quot;);"></div><img class="image-box-image-new" src="https://storage.googleapis.com/production-hostgator-brasil-v1-0-0/910/1831910/Ii0ZFo4Z/693fc155dd544bcb81e46a2c1c201f1b" width="183" height="183" style="width: 183px; height: 183px; margin-top: -1px; margin-left: 0px;"></div></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403514261" style="border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403514261"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403514261" style="width: 183px; min-height: 181px;"></div></div></div></div></a></div><div class="design-element element-size-box user-selectable-element clickable-element has-popup image-element is-section-child webzai-clickable-behaviour" id="id1719403566950" data-element-id="id1719403566950" style="left: 50%; top: 1105px; margin-left: -90px; z-index: 27;"><a class="design-element-link-part no-decorations" target="_blank" href="https://drive.google.com/drive/folders/1R9fBdYUzpxyJTfs4d02PQNkMSRA16PuG?usp=sharing"><div class="element-main-box design-element-main-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403566950" style="z-index: 27;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403566950" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-background-image design-element-background-image state-displayed image-box-new optimize-speed state-image-loaded"><div class="image-box-image-wrapper horizontal-center vertical-center stretchedToFill non-tile-layout use-image-element" style="width: 183px; height: 181px;"><div class="image-box-background-image" style="background-image: url(&quot;https://storage.googleapis.com/production-hostgator-brasil-v1-0-0/910/1831910/Ii0ZFo4Z/03c85599df6243629afefa0c977426fd&quot;);"></div><img class="image-box-image-new" src="https://storage.googleapis.com/production-hostgator-brasil-v1-0-0/910/1831910/Ii0ZFo4Z/03c85599df6243629afefa0c977426fd" width="183" height="183" style="width: 183px; height: 183px; margin-top: -1px; margin-left: 0px;"></div></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403566950" style="border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403566950"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403566950" style="width: 183px; min-height: 181px;"></div></div></div></div></a></div><div class="design-element element-size-box user-selectable-element clickable-element has-popup image-element is-section-child webzai-clickable-behaviour" id="id1719403614452" data-element-id="id1719403614452" style="left: 50%; top: 1105px; margin-left: 240px; z-index: 28;"><a class="design-element-link-part no-decorations" target="_blank" href="https://drive.google.com/drive/folders/1R9fBdYUzpxyJTfs4d02PQNkMSRA16PuG?usp=sharing"><div class="element-main-box design-element-main-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403614452" style="z-index: 28;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403614452" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-background-image design-element-background-image state-displayed image-box-new optimize-speed state-image-loaded"><div class="image-box-image-wrapper horizontal-center vertical-center stretchedToFill non-tile-layout use-image-element" style="width: 183px; height: 181px;"><div class="image-box-background-image" style="background-image: url(&quot;https://storage.googleapis.com/production-hostgator-brasil-v1-0-0/910/1831910/Ii0ZFo4Z/ad02999985b846739620eac1bb1e1e13&quot;);"></div><img class="image-box-image-new" src="https://storage.googleapis.com/production-hostgator-brasil-v1-0-0/910/1831910/Ii0ZFo4Z/ad02999985b846739620eac1bb1e1e13" width="183" height="183" style="width: 183px; height: 183px; margin-top: -1px; margin-left: 0px;"></div></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403614452" style="border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403614452"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element has-popup image-element" data-element-id="id1719403614452" style="width: 183px; min-height: 181px;"></div></div></div></div></a></div></div></div></div></div></section></div><div class="design-element element-size-box page-section-element section-element last-section last-main-section is-page-child" id="id1626822081982" data-element-id="id1626822081982"><section class="html-element page-section-element" data-element-id="id1626822081982"><div class="element-main-box design-element-main-box page-section-element" data-element-id="id1626822081982"><div class="element-background-layer element-border-target design-element-background-layer page-section-element" data-element-id="id1626822081982" style="background-color: rgb(0, 48, 97);"></div><div class="element-background-image design-element-background-image state-displayed image-box-new optimize-speed state-image-loaded"><div class="image-box-image-wrapper horizontal-center vertical-bottom stretched non-tile-layout use-image-element" style="width: 1304px; height: 300px;"><div class="image-box-background-image" style="background-image: url(&quot;https://storage.googleapis.com/wzukusers/user-500011/images/59cdef001c9f9GQeQYS1/Background-3_d1450.png&quot;);"></div><img class="image-box-image-new" src="https://storage.googleapis.com/wzukusers/user-500011/images/59cdef001c9f9GQeQYS1/Background-3_d1450.png" width="1304" height="94" style="width: 1304px; height: 94px; margin-top: 206px; margin-left: 0px;"></div></div><span class="element-overlay-layer element-border-target" style="background-color: rgba(0, 0, 0, 0.25); border-width: 0px;"></span><div class="element-border-box element-border-target element-padding-box design-element-border-box page-section-element" data-element-id="id1626822081982" style="padding: 0px; border-color: rgb(102, 102, 102); border-style: solid;"><div class="element-content-box design-element-content-box page-section-element" data-element-id="id1626822081982"><div class="content-container content-container-type element-size-box element-size-target page-section-element section-element-size-box" data-element-id="id1626822081982" style="min-height: 300px;"><div class="design-element element-size-box user-selectable-element clickable-element has-popup image-element is-section-child" id="id1623946300023" data-element-id="id1623946300023" style="left: 50%; top: 76px; margin-left: -428px; z-index: 4;"><div class="element-main-box design-element-main-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1623946300023" style="z-index: 4;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element has-popup image-element" data-element-id="id1623946300023" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-background-image design-element-background-image state-displayed image-box-new optimize-speed state-image-loaded"><div class="image-box-image-wrapper horizontal-center vertical-center stretchedToFill non-tile-layout use-image-element" style="width: 68px; height: 65px;"><div class="image-box-background-image" style="background-image: url(&quot;https://storage.googleapis.com/production-hostgator-brasil-v1-0-6/376/343376/54Hy90FZ/45d8c48ddb784fa0856fefe0b84ac60a&quot;);"></div><img class="image-box-image-new" src="https://storage.googleapis.com/production-hostgator-brasil-v1-0-6/376/343376/54Hy90FZ/45d8c48ddb784fa0856fefe0b84ac60a" width="68" height="66" style="width: 68px; height: 66px; margin-top: 0px; margin-left: 0px;"></div></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1623946300023" style="border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1623946300023"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element has-popup image-element" data-element-id="id1623946300023" style="width: 68px; min-height: 65px;"></div></div></div></div></div><div class="design-element element-size-box has-rich-content user-selectable-element clickable-element has-rich-content has-text is-section-child" id="id1626823275990" data-element-id="id1626823275990" style="left: 50%; top: 73px; margin-left: -318px; z-index: 5;"><div class="element-main-box design-element-main-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1626823275990" style="z-index: 5;"><div class="element-background-layer element-border-target design-element-background-layer has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1626823275990" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1626823275990" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1626823275990"><div class="content-container content-container-type element-size-box element-size-target has-rich-content user-selectable-element clickable-element has-rich-content has-text" data-element-id="id1626823275990" style="width: 368px; min-height: 77px;"><div class="rich-text-element-content absolute-fill element-content dir-ltr" style="background: none; text-align: left; color: rgb(251, 253, 255); line-height: 1.6; letter-spacing: 0px; font-size: 16px; font-family: &quot;Lato Light&quot;;"><div class="rich-text-positioning-wrapper vertical-alignment-top"><div class="rich-text-content common-rich-content-style has-content"><div><span style="font-size:14px;"><strong>Colégio Prima</strong></span></div><div><span style="font-size:14px;">&ZeroWidthSpace;&ZeroWidthSpace;</span><span style="font-size:12px;">Rua Dr. Milton de Souza Pacheco, 263,&ZeroWidthSpace;&nbsp;Centro,&nbsp;Maricá - RJ&ZeroWidthSpace;&ZeroWidthSpace;&ZeroWidthSpace; <br></span></div><div><span style="font-size:12px;">(021) 2634-2062&ZeroWidthSpace; ou&nbsp;96784-2704.</span><br></div></div></div></div></div></div></div></div></div><div class="design-element element-size-box user-selectable-element clickable-element has-popup image-element is-section-child webzai-clickable-behaviour" id="id1632323465036" data-element-id="id1632323465036" style="left: 50%; top: 88px; margin-left: 356px; z-index: 6;"><a class="design-element-link-part no-decorations" target="_blank" href="https://wa.me/5521967842704?text=Olá,%20estou%20vindo%20do%20site!"><div class="element-main-box design-element-main-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1632323465036" style="z-index: 6;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element has-popup image-element" data-element-id="id1632323465036" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-background-image design-element-background-image state-displayed image-box-new optimize-speed state-image-loaded"><div class="image-box-image-wrapper horizontal-center vertical-center stretchedToFill non-tile-layout use-image-element" style="width: 35px; height: 35px;"><div class="image-box-background-image" style="background-image: url(&quot;https://storage.googleapis.com/production-hostgator-brasil-v1-0-6/376/343376/54Hy90FZ/fd096b61ab9e40429d43678a20e5e579&quot;);"></div><img class="image-box-image-new" src="https://storage.googleapis.com/production-hostgator-brasil-v1-0-6/376/343376/54Hy90FZ/fd096b61ab9e40429d43678a20e5e579" width="35" height="36" style="width: 35px; height: 36px; margin-top: 0px; margin-left: 0px;"></div></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1632323465036" style="border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1632323465036"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element has-popup image-element" data-element-id="id1632323465036" style="width: 35px; min-height: 35px;"></div></div></div></div></a></div><div class="design-element element-size-box user-selectable-element clickable-element has-popup image-element is-section-child webzai-clickable-behaviour" id="id1696416689452" data-element-id="id1696416689452" style="left: 50%; top: 88px; margin-left: 294px; z-index: 7;"><a class="design-element-link-part no-decorations" target="_blank" href="https://www.instagram.com/colegioprima/"><div class="element-main-box design-element-main-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1696416689452" style="z-index: 7;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element has-popup image-element" data-element-id="id1696416689452" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-background-image design-element-background-image state-displayed image-box-new optimize-speed state-image-loaded"><div class="image-box-image-wrapper horizontal-center vertical-center stretchedToFill non-tile-layout use-image-element" style="width: 35px; height: 35px;"><div class="image-box-background-image" style="background-image: url(&quot;https://storage.googleapis.com/production-hostgator-brasil-v1-0-6/376/343376/54Hy90FZ/224bd9eda9b54f0bb18bfebcca2cdc67&quot;);"></div><img class="image-box-image-new" src="https://storage.googleapis.com/production-hostgator-brasil-v1-0-6/376/343376/54Hy90FZ/224bd9eda9b54f0bb18bfebcca2cdc67" width="35" height="35" style="width: 35px; height: 35px; margin-top: 0px; margin-left: 0px;"></div></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1696416689452" style="border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1696416689452"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element has-popup image-element" data-element-id="id1696416689452" style="width: 35px; min-height: 35px;"></div></div></div></div></a></div></div></div></div></div></section></div></div></div></div> </div></div></div></div></div></div></div></div></div></div></div><div class="footer-section page-section positioned" data-element-id="id1626439686754"></div><div class="design-element element-size-box user-selectable-element clickable-element block-element is-page-child" id="id1656955839905" data-element-id="id1656955839905" style="left: 0px; right: 0px; top: 0px; z-index: 2006;"><div class="element-main-box design-element-main-box user-selectable-element clickable-element" data-element-id="id1656955839905" style="z-index: 2006;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element" data-element-id="id1656955839905" style="background-color: rgba(251, 253, 255, 0.7);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element" data-element-id="id1656955839905" style="border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element" data-element-id="id1656955839905"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element" data-element-id="id1656955839905" style="min-height: 90px;"></div></div></div></div></div><div class="design-element element-size-box menu-element is-page-child" id="id1621122308894" data-element-id="id1621122308894" style="left: 50%; top: 24px; margin-left: -195px; z-index: 2010;"><nav class="html-element menu-element" data-element-id="id1621122308894"><div class="element-main-box design-element-main-box menu-element" data-element-id="id1621122308894" style="z-index: 2010;"><div class="element-background-layer element-border-target design-element-background-layer menu-element" data-element-id="id1621122308894" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box menu-element" data-element-id="id1621122308894" style="padding: 0px; border-color: rgb(251, 253, 255); border-style: solid;"><div class="element-content-box design-element-content-box menu-element" data-element-id="id1621122308894"><div class="content-container content-container-type element-size-box element-size-target menu-element overflow-hidden" data-element-id="id1621122308894" style="width: 675px; min-height: 40px;"><div class="absolute-fill element-content"><div class="arrangement-content-holder absolute-fill forwardLayerEvents"><span class="inline-block relative-arrangement wrap"><div class="positioned no-wrap"><span class="inline-block instance-container first-item" style="margin-left: 0px; width: 127px; height: 40px;"><div class="design-element element-size-box skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element catchLayerEvents webzai-clickable-behaviour" id="id1621122308894-id1592824224968" data-element-id="id1621122308894-id1592824224968" style="left: 0px; right: 0px; z-index: 1;"><a class="design-element-link-part no-decorations internal-link" href="http://192.168.0.134:2200/colegioprima"><div class="element-main-box design-element-main-box skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element" data-element-id="id1621122308894-id1592824224968" style="z-index: 1;"><div class="element-background-layer element-border-target design-element-background-layer skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element" data-element-id="id1621122308894-id1592824224968"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element" data-element-id="id1621122308894-id1592824224968" style="padding: 0px;"><div class="element-content-box design-element-content-box skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element" data-element-id="id1621122308894-id1592824224968"><div class="content-container content-container-type element-size-box element-size-target skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element overflow-hidden" data-element-id="id1621122308894-id1592824224968" style="min-height: 40px;"><div class="absolute-fill element-content"><span class="inline-block instance-container skin-instance-controller"><div class="design-element element-size-box template-item user-selectable-element clickable-element skin-hierarchy-box catchLayerEvents webzai-clickable-behaviour" id="id1719513251719" data-element-id="id1719513251719" style="z-index: 1;"><div class="element-main-box design-element-main-box template-item user-selectable-element clickable-element skin-hierarchy-box" data-element-id="id1719513251719" style="z-index: 1;"><div class="element-background-layer element-border-target design-element-background-layer template-item user-selectable-element clickable-element skin-hierarchy-box" data-element-id="id1719513251719" style="background-color: rgba(255, 255, 255, 0); border-width: 0px; border-radius: 0px;"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box template-item user-selectable-element clickable-element skin-hierarchy-box" data-element-id="id1719513251719" style="padding: 0px; z-index: 1; border-color: rgb(255, 255, 255); border-style: solid; border-width: 0px; border-radius: 0px; transition: none 0s ease 0s;"><div class="element-content-box design-element-content-box template-item user-selectable-element clickable-element skin-hierarchy-box" data-element-id="id1719513251719"><div class="content-container content-container-type element-size-box element-size-target template-item user-selectable-element clickable-element skin-hierarchy-box overflow-hidden" data-element-id="id1719513251719" style="min-height: 5px; border-radius: 0px;"><div class="design-element element-size-box user-selectable-element clickable-element hidden-design-element" id="id1719513251720" data-element-id="id1719513251720" style="left: -100px; top: -128px; z-index: 1;"><div class="element-main-box design-element-main-box user-selectable-element clickable-element state-hidden" data-element-id="id1719513251720" style="z-index: 1;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element" data-element-id="id1719513251720" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element" data-element-id="id1719513251720" style="border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element" data-element-id="id1719513251720"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element" data-element-id="id1719513251720" style="width: 302px; min-height: 281px;"></div></div></div></div></div><div class="design-element element-size-box user-selectable-element clickable-element has-text label-element block-element" id="id1719513251721" data-element-id="id1719513251721" style="inset: 0px; z-index: 2;"><div class="element-main-box design-element-main-box user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251721" style="z-index: 2;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251721" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251721" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251721"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251721" style="min-height: 5px;"><div class="label-element absolute-fill vertically-align-children element-content" style="overflow: hidden;"><span class="text-content element-text-container vertically-centered dir-ltr" style="overflow-wrap: break-word; text-align: center; color: rgb(0, 48, 97); line-height: 1.2; letter-spacing: 0px; font-size: 16px; font-family: &quot;Lato Light&quot;;">O Colégio Prima</span></div></div></div></div></div></div></div></div></div></div></div></span></div></div></div></div></div></a></div></span><span class="inline-block instance-container" style="margin-left: 10px; width: 127px; height: 40px;"><div class="design-element element-size-box skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element catchLayerEvents webzai-clickable-behaviour" id="id1621122308894-id1626439918620" data-element-id="id1621122308894-id1626439918620" style="left: 0px; right: 0px; z-index: 2;"><a class="design-element-link-part no-decorations internal-link" href="http://192.168.0.134:2200/segmentos"><div class="element-main-box design-element-main-box skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element" data-element-id="id1621122308894-id1626439918620" style="z-index: 2;"><div class="element-background-layer element-border-target design-element-background-layer skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element" data-element-id="id1621122308894-id1626439918620"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element" data-element-id="id1621122308894-id1626439918620" style="padding: 0px;"><div class="element-content-box design-element-content-box skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element" data-element-id="id1621122308894-id1626439918620"><div class="content-container content-container-type element-size-box element-size-target skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element overflow-hidden" data-element-id="id1621122308894-id1626439918620" style="min-height: 40px;"><div class="absolute-fill element-content"><span class="inline-block instance-container skin-instance-controller"><div class="design-element element-size-box template-item user-selectable-element clickable-element skin-hierarchy-box catchLayerEvents webzai-clickable-behaviour" id="id1719513251728" data-element-id="id1719513251728" style="z-index: 1;"><div class="element-main-box design-element-main-box template-item user-selectable-element clickable-element skin-hierarchy-box" data-element-id="id1719513251728" style="z-index: 1;"><div class="element-background-layer element-border-target design-element-background-layer template-item user-selectable-element clickable-element skin-hierarchy-box" data-element-id="id1719513251728" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box template-item user-selectable-element clickable-element skin-hierarchy-box" data-element-id="id1719513251728" style="padding: 0px; z-index: 1; border-color: rgb(255, 255, 255); border-style: solid;"><div class="element-content-box design-element-content-box template-item user-selectable-element clickable-element skin-hierarchy-box" data-element-id="id1719513251728"><div class="content-container content-container-type element-size-box element-size-target template-item user-selectable-element clickable-element skin-hierarchy-box overflow-hidden" data-element-id="id1719513251728" style="min-height: 5px;"><div class="design-element element-size-box user-selectable-element clickable-element" id="id1719513251730" data-element-id="id1719513251730"><div class="element-main-box design-element-main-box user-selectable-element clickable-element" data-element-id="id1719513251730"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element" data-element-id="id1719513251730"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element" data-element-id="id1719513251730"><div class="element-content-box design-element-content-box user-selectable-element clickable-element" data-element-id="id1719513251730"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element" data-element-id="id1719513251730"></div></div></div></div></div><div class="design-element element-size-box user-selectable-element clickable-element has-text label-element block-element" id="id1719513251731" data-element-id="id1719513251731" style="inset: 0px; z-index: 2;"><div class="element-main-box design-element-main-box user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251731" style="z-index: 2;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251731" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251731" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251731"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251731" style="min-height: 5px;"><div class="label-element absolute-fill vertically-align-children element-content" style="overflow: hidden;"><span class="text-content element-text-container vertically-centered dir-ltr" style="overflow-wrap: break-word; text-align: center; color: rgb(0, 48, 97); line-height: 1.2; letter-spacing: 0px; font-size: 16px; font-family: &quot;Lato Light&quot;;">Segmentos</span></div></div></div></div></div></div></div></div></div></div></div></span></div></div></div></div></div></a></div></span><span class="inline-block instance-container" style="margin-left: 10px; width: 127px; height: 40px;"><div class="design-element element-size-box skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element catchLayerEvents webzai-clickable-behaviour" id="id1621122308894-id1626430375538" data-element-id="id1621122308894-id1626430375538" style="left: 0px; right: 0px; z-index: 3;"><a class="design-element-link-part no-decorations internal-link" href="http://192.168.0.134:2200/pedagogico"><div class="element-main-box design-element-main-box skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element" data-element-id="id1621122308894-id1626430375538" style="z-index: 3;"><div class="element-background-layer element-border-target design-element-background-layer skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element" data-element-id="id1621122308894-id1626430375538"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element" data-element-id="id1621122308894-id1626430375538" style="padding: 0px;"><div class="element-content-box design-element-content-box skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element" data-element-id="id1621122308894-id1626430375538"><div class="content-container content-container-type element-size-box element-size-target skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element overflow-hidden" data-element-id="id1621122308894-id1626430375538" style="min-height: 40px;"><div class="absolute-fill element-content"><span class="inline-block instance-container skin-instance-controller"><div class="design-element element-size-box template-item user-selectable-element clickable-element skin-hierarchy-box catchLayerEvents webzai-clickable-behaviour" id="id1719513251737" data-element-id="id1719513251737" style="z-index: 1;"><div class="element-main-box design-element-main-box template-item user-selectable-element clickable-element skin-hierarchy-box" data-element-id="id1719513251737" style="z-index: 1;"><div class="element-background-layer element-border-target design-element-background-layer template-item user-selectable-element clickable-element skin-hierarchy-box" data-element-id="id1719513251737" style="background-color: rgba(255, 255, 255, 0); border-width: 0px; border-radius: 0px;"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box template-item user-selectable-element clickable-element skin-hierarchy-box" data-element-id="id1719513251737" style="padding: 0px; z-index: 1; border-color: rgb(255, 255, 255); border-style: solid; border-width: 0px; border-radius: 0px; transition: none 0s ease 0s;"><div class="element-content-box design-element-content-box template-item user-selectable-element clickable-element skin-hierarchy-box" data-element-id="id1719513251737"><div class="content-container content-container-type element-size-box element-size-target template-item user-selectable-element clickable-element skin-hierarchy-box overflow-hidden" data-element-id="id1719513251737" style="min-height: 5px; border-radius: 0px;"><div class="design-element element-size-box user-selectable-element clickable-element hidden-design-element" id="id1719513251738" data-element-id="id1719513251738" style="left: -100px; top: -128px; z-index: 1;"><div class="element-main-box design-element-main-box user-selectable-element clickable-element state-hidden" data-element-id="id1719513251738" style="z-index: 1;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element" data-element-id="id1719513251738" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element" data-element-id="id1719513251738" style="border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element" data-element-id="id1719513251738"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element" data-element-id="id1719513251738" style="width: 302px; min-height: 281px;"></div></div></div></div></div><div class="design-element element-size-box user-selectable-element clickable-element has-text label-element block-element" id="id1719513251739" data-element-id="id1719513251739" style="inset: 0px; z-index: 2;"><div class="element-main-box design-element-main-box user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251739" style="z-index: 2;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251739" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251739" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251739"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251739" style="min-height: 5px;"><div class="label-element absolute-fill vertically-align-children element-content" style="overflow: hidden;"><span class="text-content element-text-container vertically-centered dir-ltr" style="overflow-wrap: break-word; text-align: center; color: rgb(0, 48, 97); line-height: 1.2; letter-spacing: 0px; font-size: 16px; font-family: &quot;Lato Light&quot;;">Pedagógico</span></div></div></div></div></div></div></div></div></div></div></div></span></div></div></div></div></div></a></div></span><span class="inline-block instance-container" style="margin-left: 10px; width: 127px; height: 40px;"><div class="design-element element-size-box skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element catchLayerEvents webzai-clickable-behaviour" id="id1621122308894-id1626439686754" data-element-id="id1621122308894-id1626439686754" style="left: 0px; right: 0px; z-index: 4;"><a class="design-element-link-part no-decorations internal-link" href="http://192.168.0.134:2200/vida-escolar"><div class="element-main-box design-element-main-box skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element" data-element-id="id1621122308894-id1626439686754" style="z-index: 4;"><div class="element-background-layer element-border-target design-element-background-layer skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element" data-element-id="id1621122308894-id1626439686754"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element" data-element-id="id1621122308894-id1626439686754" style="padding: 0px;"><div class="element-content-box design-element-content-box skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element" data-element-id="id1621122308894-id1626439686754"><div class="content-container content-container-type element-size-box element-size-target skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element overflow-hidden" data-element-id="id1621122308894-id1626439686754" style="min-height: 40px;"><div class="absolute-fill element-content"><span class="inline-block instance-container skin-instance-controller"><div class="design-element element-size-box template-item user-selectable-element clickable-element skin-hierarchy-box catchLayerEvents webzai-clickable-behaviour" id="id1719513251749" data-element-id="id1719513251749" style="z-index: 1;"><div class="element-main-box design-element-main-box template-item user-selectable-element clickable-element skin-hierarchy-box" data-element-id="id1719513251749" style="z-index: 1;"><div class="element-background-layer element-border-target design-element-background-layer template-item user-selectable-element clickable-element skin-hierarchy-box" data-element-id="id1719513251749" style="background-color: rgba(255, 255, 255, 0); border-width: 0px; border-radius: 0px;"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box template-item user-selectable-element clickable-element skin-hierarchy-box" data-element-id="id1719513251749" style="padding: 0px; z-index: 1; border-color: rgb(255, 255, 255); border-style: solid; border-width: 0px; border-radius: 0px; transition: none 0s ease 0s;"><div class="element-content-box design-element-content-box template-item user-selectable-element clickable-element skin-hierarchy-box" data-element-id="id1719513251749"><div class="content-container content-container-type element-size-box element-size-target template-item user-selectable-element clickable-element skin-hierarchy-box overflow-hidden" data-element-id="id1719513251749" style="min-height: 5px; border-radius: 0px;"><div class="design-element element-size-box user-selectable-element clickable-element hidden-design-element" id="id1719513251750" data-element-id="id1719513251750" style="left: -99px; top: -129px; z-index: 1;"><div class="element-main-box design-element-main-box user-selectable-element clickable-element state-hidden" data-element-id="id1719513251750" style="z-index: 1;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element" data-element-id="id1719513251750" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element" data-element-id="id1719513251750" style="border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element" data-element-id="id1719513251750"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element" data-element-id="id1719513251750" style="width: 302px; min-height: 281px;"></div></div></div></div></div><div class="design-element element-size-box user-selectable-element clickable-element has-text label-element block-element" id="id1719513251751" data-element-id="id1719513251751" style="inset: 0px; z-index: 2;"><div class="element-main-box design-element-main-box user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251751" style="z-index: 2;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251751" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251751" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251751"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251751" style="min-height: 5px;"><div class="label-element absolute-fill vertically-align-children element-content" style="overflow: hidden;"><span class="text-content element-text-container vertically-centered dir-ltr" style="overflow-wrap: break-word; text-align: center; color: rgb(0, 48, 97); line-height: 1.2; letter-spacing: 0px; font-size: 16px; font-family: &quot;Lato Light&quot;;">Vida Escolar</span></div></div></div></div></div></div></div></div></div></div></div></span></div></div></div></div></div></a></div></span><span class="inline-block instance-container last-item" style="margin-left: 10px; width: 127px; height: 40px;"><div class="design-element element-size-box skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element catchLayerEvents webzai-clickable-behaviour" id="id1621122308894-id1626439971938" data-element-id="id1621122308894-id1626439971938" style="left: 0px; right: 0px; z-index: 5;"><a class="design-element-link-part no-decorations internal-link" href="http://192.168.0.134:2200/vemserprima"><div class="element-main-box design-element-main-box skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element" data-element-id="id1621122308894-id1626439971938" style="z-index: 5;"><div class="element-background-layer element-border-target design-element-background-layer skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element" data-element-id="id1621122308894-id1626439971938"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element" data-element-id="id1621122308894-id1626439971938" style="padding: 0px;"><div class="element-content-box design-element-content-box skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element" data-element-id="id1621122308894-id1626439971938"><div class="content-container content-container-type element-size-box element-size-target skin-element data-list-item user-selectable-element clickable-element skin-menu-button-element overflow-hidden" data-element-id="id1621122308894-id1626439971938" style="min-height: 40px;"><div class="absolute-fill element-content"><span class="inline-block instance-container skin-instance-controller"><div class="design-element element-size-box template-item user-selectable-element clickable-element skin-hierarchy-box catchLayerEvents webzai-clickable-behaviour" id="id1719513251760" data-element-id="id1719513251760" style="z-index: 1;"><div class="element-main-box design-element-main-box template-item user-selectable-element clickable-element skin-hierarchy-box" data-element-id="id1719513251760" style="z-index: 1;"><div class="element-background-layer element-border-target design-element-background-layer template-item user-selectable-element clickable-element skin-hierarchy-box" data-element-id="id1719513251760" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box template-item user-selectable-element clickable-element skin-hierarchy-box" data-element-id="id1719513251760" style="padding: 0px; z-index: 1; border-color: rgb(255, 255, 255); border-style: solid;"><div class="element-content-box design-element-content-box template-item user-selectable-element clickable-element skin-hierarchy-box" data-element-id="id1719513251760"><div class="content-container content-container-type element-size-box element-size-target template-item user-selectable-element clickable-element skin-hierarchy-box overflow-hidden" data-element-id="id1719513251760" style="min-height: 5px;"><div class="design-element element-size-box user-selectable-element clickable-element" id="id1719513251761" data-element-id="id1719513251761"><div class="element-main-box design-element-main-box user-selectable-element clickable-element" data-element-id="id1719513251761"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element" data-element-id="id1719513251761"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element" data-element-id="id1719513251761"><div class="element-content-box design-element-content-box user-selectable-element clickable-element" data-element-id="id1719513251761"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element" data-element-id="id1719513251761"></div></div></div></div></div><div class="design-element element-size-box user-selectable-element clickable-element has-text label-element block-element" id="id1719513251762" data-element-id="id1719513251762" style="inset: 0px; z-index: 2;"><div class="element-main-box design-element-main-box user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251762" style="z-index: 2;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251762" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251762" style="padding: 0px; border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251762"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element has-text label-element" data-element-id="id1719513251762" style="min-height: 5px;"><div class="label-element absolute-fill vertically-align-children element-content" style="overflow: hidden;"><span class="text-content element-text-container vertically-centered dir-ltr" style="overflow-wrap: break-word; text-align: center; color: rgb(0, 48, 97); line-height: 1.2; letter-spacing: 0px; font-size: 16px; font-family: &quot;Lato Light&quot;;">#VemSerPrima</span></div></div></div></div></div></div></div></div></div></div></div></span></div></div></div></div></div></a></div></span></div></span></div><div class="relative-child-elements-content-holder positioned forwardLayerEvents"></div></div></div></div></div></div></nav></div><div class="design-element element-size-box user-selectable-element clickable-element has-popup image-element webzai-clickable-behaviour is-page-child" id="id1621122063146" data-element-id="id1621122063146" style="left: 50%; top: 24px; margin-left: -444px; z-index: 2010;"><a class="design-element-link-part no-decorations internal-link" href="http://192.168.0.134:2200/"><div class="element-main-box design-element-main-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1621122063146" style="z-index: 2010;"><div class="element-background-layer element-border-target design-element-background-layer user-selectable-element clickable-element has-popup image-element" data-element-id="id1621122063146" style="background-color: rgba(255, 255, 255, 0);"></div><div class="element-background-image design-element-background-image state-displayed image-box-new optimize-speed state-image-loaded"><div class="image-box-image-wrapper horizontal-center vertical-center stretchedToFill non-tile-layout use-image-element" style="width: 140px; height: 40px;"><div class="image-box-background-image" style="background-image: url(&quot;https://storage.googleapis.com/production-hostgator-brasil-v1-0-6/376/343376/54Hy90FZ/6614fe5243334dbdb3703cec8203f913&quot;);"></div><img class="image-box-image-new" src="https://storage.googleapis.com/production-hostgator-brasil-v1-0-6/376/343376/54Hy90FZ/6614fe5243334dbdb3703cec8203f913" width="141" height="40" style="width: 141px; height: 40px; margin-top: 0px; margin-left: 0px;"></div></div><div class="element-border-box element-border-target element-padding-box design-element-border-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1621122063146" style="border-color: black; border-style: solid;"><div class="element-content-box design-element-content-box user-selectable-element clickable-element has-popup image-element" data-element-id="id1621122063146"><div class="content-container content-container-type element-size-box element-size-target user-selectable-element clickable-element has-popup image-element" data-element-id="id1621122063146" style="width: 140px; min-height: 40px;"></div></div></div></div></a></div></div></div></div></div></div></div>


<output id="lps-status-info">⚠️ Disconnected</output>
</body>
