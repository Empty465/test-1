![스크린샷](./testImage.jpg)
[모드팩 링크](https://www.curseforge.com/minecraft/modpacks/zero-to-engineering/, "CurseForge의 모드팩 페이지로 이동됩니다.")

# 모드팩 소개

*해당 README는 테스트 목적으로 작성되었습니다. 사실과 다를 수 있습니다.*

**최대한 마크다운 문법을 사용하기 위해 작성하였습니다.**

~~나무위키에서나 보았던 취소선~~

***
---

## Zero to Engineering

**목차**

1. 모드팩 소개
2. 모드팩 권장 사양
3. 사용된 코드 일부
4. 문의처 안내

---

### 1. 모드팩 소개

마인크래프트의 모드팩 입니다.
모드팩은 여러 모드를 조합한 패키지 형태의 2(3)차 창작물입니다.

**해당 모드팩의 목표는 자원을 모아 기계들을 구축하고, 기계들을 통해 가공한 자원을 모아서 행성을 탈출하는 목표를 가지고 있습니다.**

[Create](https://www.curseforge.com/minecraft/mc-mods/create) , [Immersive Engieering](https://www.curseforge.com/minecraft/mc-mods/immersive-engineering) 그리고 [Mekanism](https://www.curseforge.com/minecraft/mc-mods/mekanism) 모드들을 주력으로 하여 차례대로 기술 단계를 높여가는 진행 방식을 가지고 있습니다.


---

### 2. 모드팩 권장 사양

__해당 모드팩은 비쥬얼적인 요소들을 위해 Distant Horizons: A Level of Detail mod모드와 쉐이더가 적용되어 있습니다. 고사양이 아닌 하드웨어에서는 추가적인 설정을 통해 해당 기능들을 끄셔야 합니다.__

다음은 테스트한 하드웨어 사양입니다.

+ 권장 사양 (데스크탑)

  AMD 7800 3D CPU
  
  64기가 RAM
  
  RTX 5070ti GPU

+ 최소 사양 (노트북)

  i7 14세대 CPU
  
  32기가 RAM
  
  RTX 5060 GPU

---

### 3. 사용된 코드 일부
***아래 코드는 흙을 퍼내었을 때에 0.2 확률로 부싯돌을 드롭하는 코드 입니다.***
```
BlockEvents.broken(event => {
  if (event.block.id == 'minecraft:dirt') {

    if (Math.random() < 0.2) {
      event.block.popItem('minecraft:flint')
    }

  }
})
```

---


### 4. 문의처 안내

이메일: normal0308@gmail.com

디스코드: empty465

*저는 대학생 신분이기 때문에 평일 주간에는 답변이 힘들 수 있습니다.*
