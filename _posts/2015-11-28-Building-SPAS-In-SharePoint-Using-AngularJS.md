---
layout: post
title: Building SPA's in SharePoint using AngularJS
---

THIS IS WHERE THE CONTENT WILL GO...

  `render() {
    var settings = {
      dots: true,
      infinite: true,
      speed: 500,
      slidesToShow: 2,
      slidesToScroll: 2
    };
    return (
      <div className="component-container">
        <div className={styles.slider}>
          <Slider {...settings}>
            {this
              .props
              .alerts
              .map(function (alert, index) {
                return (
                  <div key={'alert-' + index}>
                    <AlertsItem item={alert}/>
                  </div>
                );
              })
            }
          </Slider>
        </div>
      </div>
    );`
