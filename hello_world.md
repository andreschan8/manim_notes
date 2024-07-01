# Manim Begins

I'm writing these docs to record part of my learning path using manim. I'll only include what I consider necessary. Let's start with the first experiment.

# 1. First Experiment
I installed manim some while ago and achieved to print LaTex formulas on screen. Today I changed the background color (which was unbearably confusing). This is the python file:
```python
from manim import *

class hello(Scene):
    def construct(self):
    
        self.camera.background_color = '#8A8340'
        
        text = '''
            \\begin{equation}
                \int_{0}^{\infty} f(x)dx=0
            \\end{equation}
        '''
        self.play(Write(Tex(text)))
        self.wait(3)
```
