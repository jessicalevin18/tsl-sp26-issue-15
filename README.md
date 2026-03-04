## TSL Spring 2026 Issue 15

#### Visualizations


____________________________________________

### TSL Data Desk Formatting Guidelines

#### Set all fonts to Palatino
```
theme(text = element_text(family = "Palatino"))
```

#### Clear gridlines for black and white copy
```
theme(panel.grid.major = element_blank(),
      panel.grid.minor = element_blank())
```

#### Color Guidelines

##### Online version
Any variation of colors you think look good works!

##### Black and white print version
Any grayscale colors work as long as they will be distinguishable in print. For ex: 
```
b_w <- c("label1" = "#666666", "label2= "#666666", "label3"= "#999999", "label4"= "#CCCCCC")
```

#### Other theme guidelines
```
theme_minimal() +
theme(axis.title.x = element_text(margin = margin(t = 15)),
        axis.title.y = element_text(margin = margin(r = 10)))
```

#### Export code
```
ggsave("ai-professor-policy-bw-nolines.pdf", plot = b_w_no_lines, device = "pdf", width = 8, height = 6)
