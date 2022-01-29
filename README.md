# cython_bbox

cython_bbox is widely used in object detection tasks. To my best knowledge, it was first implemented in [Faster-RCNN](https://github.com/rbgirshick/py-faster-rcnn). Since then, almost all object detection projects use the source code directly.

In order to use it in standalone code snippets or small projects, Yanfeng Liu made it a pypi module (https://github.com/yanfengliu/cython_bbox.git). The `cython_bbox.pyx` is totally borrowed from [Faster-RCNN](https://github.com/rbgirshick/py-faster-rcnn). Thanks [RBG](http://www.rossgirshick.info/)!

This repo appends additional bounding box intersection feature to Yanfeng Liu's version of cython_bbox.

## install

from `../cython_bbox/` type

```
pip install .
```

## usage


```
from cython_bbox import bbox_overlaps
overlaps = bbox_overlaps(
        np.ascontiguousarray(dt, dtype=np.float32),
        np.ascontiguousarray(gt, dtype=np.float32)
    )

```
