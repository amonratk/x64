# How to set border style to cell

## Defined style

```bash
$styleArray = array(
    'borders' => array(
        'allborders' => array(
            'style' => PHPExcel_Style_Border::BORDER_THIN
        )
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
