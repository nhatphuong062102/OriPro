# OriPro
Đây là phiên bản gốc nhưng đã tách flag `is_bonder` và `use_refined`

Nếu có vấn đề thì xóa hết flag mới ở cả hai nơi **OriPro** và **MyProject** và BẬT `--is_bonder True` ở file `eval.sh`

**OriPro** có description giống hệt **MyProject**. Nếu có vấn đề thì: dùng lại `BTXRD-old.json`

**OriPro** có transform giống hệt **MyProject**. Nếu có vấn đề thì:
* Xóa `RRCROP_SCALE` --- dành cho phần **train**
* (1) Xóa `_build_transform_test()` hiện tại, dùng bản `_build_transform_test()` cũ đang được cmt; (2) Xóa `test()` và `test_ood()` hiện tại, dùng bản `test()` và `test_ood()` cũ đang được cmt  --- dành cho phần **test**

**OriPro** có các hyperparameter giống hệt **MyProject**. Nếu có vấn đề thì: Xóa `OPTIM` hiện tại, dùng bản `OPTIM` cũ đang được cmt