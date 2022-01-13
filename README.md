# ColorBoard

> 该项目为 Shore Design System 的标准色板、文字排版 Token 文件

## 格式说明

对象名为描述样式的名称，“/”描述层级关系，如果无层级关系可忽略，只保留最后一个“/”后的文本。

### "type": "SOLID"

`"type": "SOLID"` 为填充样式，暂时只有色彩填充，未来可能会包含渐变色填充。

色彩的 Alpha 通道

```

"opacity": 1,

```

色彩 RGB

```

"color": {

  "r": 0.6285256743431091,
  "g": 0.25052082538604736,
  "b": 0.925000011920929
  
}

```

iOS 直接使用 RGB 值可支持 P-3 色域表现，Web 需转换为，256进制的 rgba() 格式

### type": "TEXT"

`type": "TEXT"` 为文本样式，包含字体、字号、字重、字间距。

字体家族与字重

```

"fontname": {

  "family": "Shore UI",
  "style": "Regular"
  
}

```

字号

```

"fontsize": 17

```

行高

```

"lineheight": {
  "unit": "PIXELS",
  "value": 24
}

```

字间距

```

"letterspacing": {
  "unit": "PERCENT",
  "value": -0.008999999612569809
}

```

"unit" 为 value 描述的单位
