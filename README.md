**1. Clone wallet sources**

```
git clone https://github.com/unclevito2017/Monkey-Balls.git
```

**2. Modify `CryptoNoteWallet.cmake`**
 
```
set(CN_PROJECT_NAME "Monkey-Balls")
set(CN_CURRENCY_DISPLAY_NAME "Monkey Balls")
set(CN_CURRENCY_TICKER "MBS")
```

**3. Set symbolic link to coin sources at the same level as `src`. For example:**

```
ln -s ../cryptonote cryptonote
```

Alternative way is to create git submodule:

```
git submodule add https://github.com/unclevito2017/Monkey-Balls.git MonkeyBalls
```

Replace URL with git remote repository of your coin.

**4. Build**

```
mkdir build && cd build && cmake .. && make
```
