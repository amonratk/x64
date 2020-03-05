# How to set backgroud color style to cell

## Defined style

```bash
$styleArray = array(
    'fill' => array(
        'type' => PHPExcel_Style_Fill::FILL_SOLID,
        'startcolor' => array('rgb' => '96faf8')
    )
);
```

## Instanace

```bash
$objPHPExcel = new PHPExcel();
$objPHPExcel->setActiveSheetIndex(0);
$sheet = $objPHPExcel->getActiveSheet();
```

## Set style to cell

```bash
$sheet->getStyle('A3:M3')->applyFromArray($styleArray);
```
