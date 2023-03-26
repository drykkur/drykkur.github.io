---
layout: post
title:  "Welcome to Jekyll!"
date:   2023-03-26 13:33:49 +0200
categories: jekyll update
---
þetta er texti


{% highlight python %}
polardf = data_focus.copy()
polardf = polardf[polardf.Category == 'PROSTITUTION']
polardata = polardf.groupby(['Hour','Category']).size().to_frame().reset_index()
polardata.rename(columns={0: 'CrimeCount'}, inplace=True)
fig = go.Figure(go.Barpolar(
    r=polardata.CrimeCount,
    marker_color=px.colors.qualitative.Light24,
    marker_line_color='black',
    marker_line_width=2,
    opacity=0.8,
))

fig.update_layout(
    template=None,
    polar = dict(
        radialaxis = dict(range=[0, 1575], angle=70, tickangle=90, ticklabelstep=1, tickvals = [600,800,1000,1200,1400]),
        angularaxis = dict(showticklabels=True, ticks='', direction='clockwise', tickvals = [0,45,90,135,180,225,270,315], ticktext=['00','03','06','09','12','15','18','21'])
    )
)
fig.show()
{% endhighlight %}

![test](/assets/resilar.jpg){:class="img-responsive"}


