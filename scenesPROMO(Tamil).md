# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[PLAY!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: நாங்கள் தொடங்குவதற்கு முன், *நீங்கள்* எப்படி படிக்க விரும்புகிறீர்கள்?

`publish("show_options_bottom")`

# intro-start-2

n3: இப்போது நம் கதையை ஆரம்பிக்கலாம்...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: இது ஒரு மனிதன்

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

n: மேலும் இது மனிதனின் கவலை

n: _நீ_ தான் கவலை

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: இல்லை. இல்லை, இல்லை, கேட்கவில்லை. என் போனை பார்க்கிறேன்.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: உங்கள் மனிதனை பாதுகாப்பதே உங்கள் பணி *DANGER*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: மூச்சுத்திணறல்! ட்விட்டரில் உங்கள் வாழ்க்கையை ஸ்க்ரோல் செய்கிறீர்கள்! மீண்டும்!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: ஆமாம், நான் ஏன் என் எண்ணங்களை அடிக்கடி உட்கார்ந்து கேட்கவில்லை என்று எனக்கு ஆச்சரியமாக இருக்கிறது.
`hong({eyes:"neutral"});`

n: சீக்கிரம், ஏ பற்றி எச்சரிக்கவும் *DANGER!*

```
bb({eyes:"look"});
```

[அடடா, அந்த பயங்கரமான செய்தியைப் பாருங்கள்!](#act1d_news)

[இல்லை, அந்த ட்வீட் ரகசியமா?*us?*](#act1d_subtweet)

[ஏய், பூனை பால் குடிக்கும் GIF](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: ஹாய் அது அழகாக இருக்கிறது, நான்-

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: **பூனைகளால் பாலை ஜீரணிக்க முடியாது மற்றும் விலங்குகளை துன்புறுத்துவதை அனுபவிக்கும் பயங்கரமான மனிதர்கள் நாங்கள்**

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



