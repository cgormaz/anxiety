# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[PLAY!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Antes de que empecemos, ¿cómo te gustaría leer?

`publish("show_options_bottom")`

# intro-start-2

n3: Bien, comencemos nuestra historia...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: ESTE ES UN HUMANO

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: Y ESTA ES LA ANSIEDAD DE ESE HUMANO

n: _TÚ_ ERES LA ANSIEDAD

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Nop. No, nop, no te escucho. Voy a revisar mi teléfono.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: TU TRABAJO ES PROTEGER A TU HUMANO DEL *PELIGRO*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: ¡Oh no! ¡Estás desperdiciando tu vida en Twitter! ¡De nuevo!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Sí, me pregunto por qué no me siento a escuchar mis pensamientos más seguido.

`hong({eyes:"neutral"});`

n: ¡RÁPIDO, ADVIÉRTELES SOBRE EL *PELIGRO!*

```
bb({eyes:"look"});
```

[¡Oh no, mira esta horrible noticia!](#act1d_news)

[Oh no, is that tweet secretly about *us?*](#act1d_subtweet)

[Hey, a GIF of a cat drinking milk](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Heh ya that's cute, I--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: CATS CAN'T DIGEST MILK AND WE'RE TERRIBLE PEOPLE FOR ENJOYING ANIMAL ABUSE

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



