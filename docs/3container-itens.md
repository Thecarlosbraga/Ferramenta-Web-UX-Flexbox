# 🏗️ Propriedades do Container e Itens

No Flexbox, existe uma **hierarquia clara** entre **Container** e **Itens**, que define como as propriedades afetam o layout:

## 💠 Hierarquia de Propriedades

### Container (Pai)
- `justify-content` → alinha os itens no **eixo principal**  
- `align-items` → alinha os itens no **eixo transversal**  
- `flex-direction` → define a **direção dos itens**

### Itens (Filho)
- `flex-grow` → controla o **crescimento relativo**  
- `flex-shrink` → controla o **encolhimento relativo**  
- `align-self` → sobrescreve `align-items` para o item específico

## 🌀 Representação Visual
```
+------------------+
| Container |
| justify-content |
| align-items |
| flex-direction |
+------------------+
|
v (Hierarquia)
+------------------+
| Itens |
| flex-grow |
| flex-shrink |
| align-self |
+------------------+
```
