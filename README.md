# kivy-amlak
import kivy
kivy.require('1.0.7')

from kivy.app import App
from kivy.uix.floatlayout import FloatLayout
from kivy.uix.slider import Slider
from kivy.graphics import Color, Bezier, Line
from kivy.uix.button import Button
from kivy.uix.boxlayout import BoxLayout
from kivy.uix.label import Label
from kivy.graphics import Rectangle, Color
class amlakApp(App):
    def build(self):
        box = FloatLayout()
        with box.canvas:
            Rectangle(source="C:/Users/orzhans%20system/Desktop/mahdi.jpg",size_hint=(0.2,0.1),pos=(470,540))
        def on_focus(instance, value):
            instance.text = ""
        b = Label(text="SALAM SHOMA MITOONID BA ZADAN ROOYE LINK ZIR VARED SHABAKE HA SHAVID",size_hint=(0.1 , 0.1),pos=(460,420))
        box.add_widget(b)
        d = Button(text="SAIT MA",size_hint=(0.2, 0.1),pos=(430,300))
        box.add_widget(d)
        c = Button(text="KANAL TELEGRAM",size_hint=(0.2, 0.1),pos=(430,233))
        box.add_widget(c)
        e = Button(text="EMAIL MA",size_hint=(0.2, 0.1),pos=(430,167))
        box.add_widget(e)
        return box



    

if __name__ == '__main__':
   amlakApp().run()
