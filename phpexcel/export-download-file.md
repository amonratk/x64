# How to set header for download file

## Instance

```bash
$objPHPExcel = new PHPExcel();
```

and more detail of `$objPHPExecl`

## Defined filename

```bash
$fileName = 'Summary_Estimated_'.date('YmdHis').'.xlsx';
```

## Save file to disk

```bash
$filepath = './files/'.$fileName;
$objWriter = new PHPExcel_Writer_Excel2007($objPHPExcel);
$objWriter->save($filepath);
```

## Make to file for download

```bash
header('Content-Type: application/vnd.openxmlformats-officedocument.spreadsheetml.sheet');
header('Content-Disposition: attachment;filename="'.$fileName.'"');
header('Cache-Control: max-age=0');
header('Cache-Control: max-age=1');

header ('Expires: Mon, 26 Jul 1997 05:00:00 GMT');
header ('Last-Modified: '.gmdate('D, d M Y H:i:s').' GMT');
header ('Cache-Control: cache, must-revalidate');
header ('Pragma: public');

$objWriter = PHPExcel_IOFactory::createWriter($objPHPExcel, 'Excel2007');
$objWriter->save('php://output');
exit;
```
