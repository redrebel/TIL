기본으로 입력하는 초기 임포트  

```python
from IPython.display import display
import numpy as np
import matplotlib.pyplot as plt
import pandas as pd
import mglearn
```
```%matplotlib inline```
```python
import matplotlib.font_manager as fm
# 사용가능한 폰트확인
fm.get_fontconfig_fonts()
font_location = "/Library/Fonts/AppleGothic.ttf"
font_name = fm.FontProperties(fname=font_location).get_name()
matplotlib.rc('font', family=font_name)
```
