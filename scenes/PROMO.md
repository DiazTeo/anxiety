# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[PLAY!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Donc avant de commencer, comment aimeriez *vous* lire ?

`publish("show_options_bottom")`

# intro-start-2

n3: Now, let's begin our story...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: VOICI UN HUMAIN!

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

n: ET VOICI L'ANXIETE DE L'HUMAIN

n: _VOUS_ ETES L'ANXIETE

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Non. non, pas encore, je ne t'ecouterais pas. Je prefere regarder mon telephone.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: VOTRE TRAVAIL EST DE PROTEGER VOTRE HUMAIN DU *DANGER*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: QUOI! Tu gaches ta vie sur Twitter ! Encore !

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Oui, je me demande pourquoi je ne me pose pas plus souvent pour ecouter mes pensee.

`hong({eyes:"neutral"});`

n: VITE, AVERTI LES A PROPOS D'UN *DANGER!*

```
bb({eyes:"look"});
```

[Oh non, regarde cette horrible histoire!](#act1d_news)

[Oh non, est ce que ce tweet parle secretement de *nous* ?](#act1d_subtweet)

[Regarde, un GIF de chat buvant du lait](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: En Effet, c'est plutot mignon, je--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: LES CHATS NE PEUVENT PAS DIGERER LE LAIT ET NOUS SOMMES DES GENS HORRIBLE QUI AIMONS LA MALTRAITANCE ANIMAL

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



