---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

清孙温绘全本红楼梦图（A Dream of Red Mansions As portrayed through the brush of Sun Wen）是清代画家孙温所创作的一幅绢本工笔彩绘画

A series of paintings on silk, telling the story of Hong Lou Meng (A Dream of Red Mansions), a famous Chinese literary classic.

前往 [github 仓库](https://github.com/changren-wcr/sunwen) 下载高清图片

go to [github repo](https://github.com/changren-wcr/sunwen) to download full-resolution images

{% for image in site.static_files %}
{% if image.path contains 'sunwen' %}

<figure>
<img src="{{ site.baseurl }}{{ image.path }}" alt={{image.basename}} />

<figcaption>{{image.basename}}</figcaption>
</figure>

{% endif %}
{% endfor %}
