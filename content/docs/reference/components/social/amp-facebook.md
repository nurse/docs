---
$title: amp-facebook
$order: 26
---

<!---
Copyright 2015 The AMP HTML Authors. All Rights Reserved.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

      http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS-IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
-->



<table>
  <tr>
    <td width="40%"><strong>Description</strong></td>
    <td>Displays a Facebook post or video. </td>
  </tr>
  <tr>
    <td width="40%"><strong>Availability</strong></td>
    <td>Stable</td>
  </tr>
  <tr>
    <td width="40%"><strong>Required Script</strong></td>
    <td><code>&lt;script async custom-element="amp-facebook" src="https://cdn.ampproject.org/v0/amp-facebook-0.1.js">&lt;/script></code></td>
  </tr>
  <tr>
    <td class="col-fourty"><strong><a href="https://www.ampproject.org/docs/guides/responsive/control_layout.html">Supported Layouts</a></strong></td>
    <td>fill, fixed, fixed-height, flex-item, nodisplay, responsive</td>
  </tr>
  <tr>
    <td width="40%"><strong>Examples</strong></td>
    <td><a href="https://ampbyexample.com/components/amp-facebook/">Annotated code example for amp-facebook</a></td>
  </tr>
</table>
## Overview 

You can use the `amp-facebook` component to embed a Facebook post or a Facebook video.

**Example: Embedding a post**

[sourcecode:html]
<amp-facebook width=486 height=657
    layout="responsive"
    data-href="https://www.facebook.com/zuck/posts/10102593740125791">
</amp-facebook>
[/sourcecode]

**Example: Embedding a video**

[sourcecode:html]
<amp-facebook width=552 height=574
    layout="responsive"
    data-embed-as="video"
    data-href="https://www.facebook.com/zuck/videos/10102509264909801/">
</amp-facebook>
[/sourcecode]

## Attributes

**data-href** (required)

The URL of the Facebook post/video. For example: https://www.facebook.com/zuck/posts/10102593740125791.

**data-embed-as** (optional)

The value is either `post` or `video`.  The default is `post`.

Both posts and videos can be embedded as a post. Setting `data-embed-as="video"` for Facebook videos only embeds the player of the video, and ignores the accompanying post card with it. This is recommended if you'd like a better aspect ratio management for the video to be responsive.  

Check out the documentation for differences between [post embeds](https://developers.facebook.com/docs/plugins/embedded-posts) and [video embeds](https://developers.facebook.com/docs/plugins/embedded-video-player).

**common attributes**

This element includes [common attributes](https://www.ampproject.org/docs/reference/common_attributes) extended to AMP components.

## Validation

See [amp-facebook rules](https://github.com/ampproject/amphtml/blob/master/extensions/amp-facebook/0.1/validator-amp-facebook.protoascii) in the AMP validator specification.