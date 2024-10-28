# INTELIGÊNCIA DE TEMPO

## Criando tabela dCalendar

### - DateMin

```
= List.Min(fTABELA[date])
```

### - DateMax

```
= List.Max(fTABELA[date])
```

### - Range

```
= Duration.Days( DateMax - DateMin) + 1
```

### - ListDate

```
= List.Dates(DateMin, Range, #duration(1,0,0,0))
```

### 1. Obs: Converter para tabela e valores para tipo 'Date'.

### 2. Obs: Inserir coluna para Ano (Int) e Mês (Int).

### 3. Obs: Inserir coluna 'ID'.

---

## Criando Tabela dMonths

### Selecionar Mes (Int) excluir outras colunas.

### Tabela de meses
```
= Table.Distinct(#"Outras Colunas Removidas", {"Mês"})
```

### 1. Obs: Classificar por Mês (Int)

```
- Power BI
→ Ferramentas da coluna
→ Classificar por coluna

# Classificar por coluna Mês (Int).
```




---

<img src="../src/power-bi.svg" alt="Power BI Logo" style="height: 100px;">
