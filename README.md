# 代数学

## 主要内容

Bourbaki《数学原本》(Éléments de mathématique) 中《代数学》一卷的自学笔记。

## 说明

本笔记按 Bourbaki 原书的章节层级组织，对应关系如下：

| Bourbaki 原书 | 本笔记 | 本仓库中的示例 |
|---|---|---|
| 章（Chapitre） | `Content/` 下的**章目录** | `1_Description_of_Formal_Mathematic/` |
| 节（§） | 章目录下的**节目录** | `1_Terms_and_relations/` |
| 小节（1、2、…） | 节目录下的 **`.tex` 文件** | `1_signs_and_assembiles.tex` |

- 目录与文件名取该层级标题的**英译**，并加编号前缀（`1_`、`2_`…，不加前导零）。
- 中文标题写在 `\chapter{...}` 与 `\section{...}` 中：`\chapter{}` 用该**节目录**名的中译，`\section{}` 用该**文件**名的中译。
- 每层目录各有一个 `index.tex`，按顺序汇总对下一层的 `\input`。

定理环境用法、交叉引用（`\cref`）、符号库维护等 **tex 层面的规定**，另见模板《笔记写作》的 README。

## 内容结构

```
Content/
├─ 1_Description_of_Formal_Mathematic/
│  ├─ 1_Terms_and_relations/
│  ├─ 2_Theorems/
│  ├─ 3_Logical_theories/
│  ├─ 4_Quantified_theories/
│  ├─ 5_Equalitarian_theories/
│  └─ Appendix_Characterization_of_terms_and_relations/
├─ 2_Set_Theory/
│  ├─ 1_Collectivizing_relations/
│  ├─ 2_Ordered_pairs/
│  ├─ 3_Correspondence/
│  ├─ 4_Union_and_intersection_of_a_family_of_sets/
│  ├─ 5_Product_of_a_family_of_sets/
│  └─ 6_Equivalence_relations/
├─ 3_Ordered_Sets_Cardinals_Natural_Numbers/
│  ├─ 1_Ordered_relations_Ordered_sets/
│  ├─ 2_Well_ordered_sets/
│  ├─ 3_Equipotent_sets_cardinals/
│  ├─ 4_Natural_numbers_Finite_sets/
│  ├─ 5_Properties_of_natural_numbers/
│  ├─ 6_Infinite_sets/
│  └─ 7_Inverse_limits_and_direct_limits/
├─ 4_Algebraic_Structure/
│  ├─ 1_Laws_of_composition_associativity_commutativity/
│  ├─ 2_Idendity_element_cancellable_elements_invertible_elements/
│  ├─ 3_Actions/
│  ├─ 4_Groups_and_groups_with_operators/
│  ├─ 5_Groups_operating_on_a_set/
│  ├─ 6_Extension_solvable_groups_nilpotent_groups/
│  ├─ 7_Free_monoids_free_groups/
│  ├─ 8_Rings/
│  ├─ 9_Division_rings/
│  └─ 010_Inverse_and_direct_limits/
├─ 5_Linear_Algebra/
│  ├─ 1_Modules/
│  ├─ 2_Modules_of_linear_mappings_Duality/
│  ├─ 3_Tensor_product/
│  ├─ 4_Relations_between_tensor_products_and_homomorphism_modules/
│  ├─ 5_Extension_of_the_rings_of_scalars/
│  ├─ 6_Inverse_and_direct_limits_of_modules/
│  ├─ 7_Vector_spaces/
│  ├─ 8_Restrictions_of_the_division_ring_of_scalars_in_vector_spaces/
│  ├─ 9_Affine_spaces_and_projective_spaces/
│  ├─ 010_Matrices/
│  ├─ 011_Graded_modules_and_rings/
│  └─ Appendix_Pseudomodules/
├─ 6_Tensor_Algebra_Exterior_Algebra_Symmetric_Algebra/
│  ├─ 1_Algebras/
│  ├─ 2_Examples_of_algebras/
│  ├─ 3_Graded_algebras/
│  ├─ 4_Tensor_products_of_algebras/
│  ├─ 5_Tensor_algebra_tensors/
│  ├─ 6_Symmetric_algebras/
│  ├─ 7_Exterior_algebras/
│  ├─ 8_Determinants/
│  ├─ 9_Norms_and_traces/
│  ├─ 010_Derivations/
│  ├─ 011_Coalgebras_products_of_multilinear_forms_inner_products_and_duality/
│  └─ Appendix_Altenative_algebras_octonions/
├─ 7_Polynomials_and_Rational_Fractions/
│  ├─ 1_Polynomials/
│  ├─ 2_Zeros_of_polynomials/
│  ├─ 3_Rational_fractions/
│  ├─ 4_Formal_power_series/
│  ├─ 5_Symmetric_tensors_and_polynomial_mappings/
│  └─ 6_Symmetric_functions/
├─ 8_Fields_Theory/
│  ├─ 1_Prime_fields_Characteristic/
│  ├─ 2_Extensions/
│  ├─ 3_Algebraic_extensions/
│  ├─ 4_Algebraically_closed_extensions/
│  ├─ 5_p-radical_extensions/
│  ├─ 6_Etale_algebra/
│  ├─ 7_Separable_algebraic_extensions/
│  ├─ 8_Norms_and_traces/
│  ├─ 9_Conjugate_elements_and_quasi-Galois_extensions/
│  ├─ 10_Galois_extensions/
│  ├─ 11_Abelian_extensions/
│  ├─ 12_Finite_fields/
│  ├─ 13_p-radical_extensions_of_height_≤_1/
│  ├─ 14_Transcendental_extensions/
│  ├─ 15_Separable_extensions/
│  ├─ 16_Differential_criteria_of_separability/
│  └─ 17_Regular_extensions/
├─ 9_Ordered_Groups_and_Fields/
│  ├─ 1_Ordered_groups_Divisibility/
│  └─ 2_Ordered_fields/
├─ 10_Modules_over_Principal_Ideal_Domains/
│  ├─ 1_Principal_ideal_domains/
│  ├─ 2_Torsion_modules_over_a_principal_ideal_domain/
│  ├─ 3_Free_modules_over_a_principal_ideal_domain/
│  ├─ 4_Finitely_generated_modules_over_a_principal_ideal_domain/
│  └─ 5_Endomorphisms_of_vector_spaces/
├─ 11_Semisimple_Modules_and_Rings/
│  ├─ 1_Artinian_Modules_and_Noetherian_Modules/
│  ├─ 2_The_Structure_of_Modules_of_Finite_Length/
│  ├─ 3_Simple_Modules/
│  ├─ 4_Semisimple_Modules/
│  ├─ 5_Commutation/
│  ├─ 6_Morita_Equivalence_of_Modules_and_Algebras/
│  ├─ 7_Simple_Rings/
│  ├─ 8_Semisimple_Rings/
│  ├─ 9_Radical/
│  ├─ 10_Modules_over_an_Artinian_Ring/
│  ├─ 11_Grothendieck_Groups/
│  ├─ 12_Tensor_Products_of_Semisimple_Modules/
│  ├─ 13_Absolutely_Semisimple_Algebras/
│  ├─ 14_Central_Simple_Algebras/
│  ├─ 15_Brauer_Groups/
│  ├─ 16_Other_Descriptions_of_the_Brauer_Group/
│  ├─ 17_Reduced_Norms_and_Traces/
│  ├─ 18_Simple_Algebras_over_a_Finite_Field/
│  ├─ 19_Quaternion_Algebras/
│  ├─ 20_Linear_Representations_of_Algebras/
│  ├─ 21_Linear_Representations_of_Finite_Groups/
│  ├─ Appendix_01_Algebras_without_Unit_Element/
│  ├─ Appendix_02_Determinants_over_a_Noncommutative_Field/
│  ├─ Appendix_03_Hilberts_Nullstellensatz/
│  └─ Appendix_04_Trace_of_an_Endomorphism_of_Finite_Rank/
├─ 12_Sesquilinear_Forms_and_Quadratic_Forms/
│  ├─ 1_Sesquilinear_forms/
│  ├─ 2_Discriminant_of_a_sesquilinear_form/
│  ├─ 3_Hermitian_forms_and_quadratic_forms/
│  ├─ 4_Totally_isotropic_subspaces_Witts_theorem/
│  ├─ 5_Special_properties_of_alternating_bilinear_forms/
│  ├─ 6_Special_properties_of_hermitian_forms/
│  ├─ 7_Hermitian_forms_and_ordered_fields/
│  ├─ 8_Types_of_quadratic_forms/
│  ├─ 9_Clifford_algebras/
│  └─ 10_Angles/
└─ 13_Homological_Algebra/
   ├─ 1_Complements_of_linear_algebra/
   ├─ 2_Complexes_of_A-modules/
   ├─ 3_Resolutions/
   ├─ 4_Torsion_products/
   ├─ 5_Modules_of_extensions/
   ├─ 6_Use_of_non-canonical_resolutions/
   ├─ 7_Composition_product/
   ├─ 8_Homological_dimension/
   └─ 9_Koszul_complexes/
```

## 文件结构

```
main.tex          编译入口
structure.sty     样式包：页面设置、定理环境、引用、数学符号库
quiver.sty        交换图支持
Content/          分章正文，每章一个目录，由 index.tex 汇总 \input
commit.py         一键提交并推送（说明见 commit.md）
setup_mode.py     习题编排模式切换（说明见 setup_mode.md）
README.md         本文件：项目说明
CHANGELOG.md      更新日志：tex 配置调整与正文内容调整
```

各脚本的选项与功能分别见 [commit.md](commit.md) 与 [setup_mode.md](setup_mode.md)；符号库由上层目录的 `symbols.py` 统一管理。

## 编译

本笔记使用自建的【笔记写作】模板（样式包 `structure.sty`），须用 **XeLaTeX** 编译：

```bash
xelatex main.tex
```

- **编译环境**：XeLaTeX。模板依赖 ctexbook 与 XeLaTeX 特性，**不支持 pdfLaTeX**。
- **TeXStudio**：建议 4.0 或更高版本。
- `main.pdf` 未纳入版本控制，需本地编译生成。
