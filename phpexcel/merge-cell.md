# How to merge cell of PHPExcel

## Instance

```bash
$objPHPExcel = new PHPExcel();
$objPHPExcel->setActiveSheetIndex(0);
$sheet = $objPHPExcel->getActiveSheet();
```

## Merge cell of A2 to M2

```bash
$sheet->mergeCells('A2:M2');
```