![스크린샷](./testImage.jpg)
[모드팩 링크](https://www.curseforge.com/minecraft/modpacks/zero-to-engineering/, "CurseForge의 모드팩 페이지로 이동됩니다.")

# 모드팩 소개

*해당 README는 테스트 목적으로 작성되었습니다. 사실과 다를 수 있습니다.*

**최대한 마크다운 문법을 사용하기 위해 작성하였습니다.**

~~나무위키에서나 보았던 취소선~~

***
---

## Zero to Engineering

1. 모드팩 소개
2. 모드팩 권장 사양
3. 사용된 코드 일부
4. 문의처 안내

---

### 4. 사용된 코드 일부
***아래 코드는 흙을 퍼내었을 때에 0.2 확률로 부싯돌을 드롭하는 코드 입니다.***
```BlockEvents.broken(event => {
  if (event.block.id == 'minecraft:dirt') {

    if (Math.random() < 0.2) {
      event.block.popItem('minecraft:flint')
    }

  }
})
```
