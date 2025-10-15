# 📘 Conceitos Fundamentais

Antes de entrarmos nas propriedades do Flexbox, existe um **seletor importante** que vale a pena conhecer: o **seletor global `*`**.

O seletor global `*` em CSS corresponde a **todos os elementos do documento**.  
Ele é muito útil para **resets** e **normalizações rápidas**, mas use com cuidado:  
aplicar propriedades pesadas no `*` pode causar **heranças inesperadas** e **sobrescritas**, dificultando a manutenção. Sempre que possível, **limite o escopo**.

```css
*, *::before, *::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

+------------------------+
|      Flex Container    |
|  +---+ +---+ +---+    |
|  |Itm| |Itm| |Itm|    |
+------------------------+
Eixo Principal -->
Eixo Transversal ↑
