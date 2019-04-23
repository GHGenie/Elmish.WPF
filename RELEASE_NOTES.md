#### 2.0.0

* No changes, but updated for Elmish 3.0 so the package can finally move out of beta

#### 2.0.0-beta-11

* Add Binding.subModelSelectedItem

#### 2.0.0-beta-10

* Fix checkboxes erroneously being shown as failing validation (#78) by @BillHally
* The above fix also fixes binding warnings for two-way bindings

#### 2.0.0-beta-9

* Add new bindings `oneWayOpt` and `twoWayOpt` ([#75](https://github.com/elmish/Elmish.WPF/issues/75))
* Update to Elmish 3.0.0-beta-7

#### 2.0.0-beta-8

* Add new binding `subBindingSeq`, see readme for details.

#### 2.0.0-beta-7

* Fix Elmish dependency version in nuget spec

#### 2.0.0-beta-6

* Update to Elmish 3
* Dispatch on UI thread to block instead of getting weird UI behaviour from race conditions when updates take too long

#### 2.0.0-beta-5

* Fix `subModelSeq` items  being unselected during updates

#### 2.0.0-beta-4

* Breaking: Change order of `oneWayLazyWith` arguments to and rename it to `oneWayLazy`, removing the existing `oneWayLazy` function. The rationale is explained in [#60](https://github.com/elmish/Elmish.WPF/issues/60) . To migrate from 2.0.0-beta-3 to 2.0.0-beta-4: Add `(=)` as the `equals` parameter to `oneWayLazy` usages, and rename `oneWayLazyWith` usages to `oneWayLazy`.
* Add `Binding.oneWaySeqLazy`

#### 2.0.0-beta-3

* Add convenience function to create design-time VMs

#### 2.0.0-beta-2

* Improve log messages

#### 2.0.0-beta-1

* Complete rewrite, several breaking changes and new features
* `twoWayValidation` is called `twoWayIfValid` (because that’s what it is, and it clearly separates it from the new `twoWayValidate`)
* `oneWayMap` is called `oneWayLazy` (its implementation has changed, and the use case has expanded, but is similar)
* `cmd` and `cmdIf` have been renamed `paramCmd` and `paramCmdIf`, because the old names have new signatures/use-cases
* `model` has been renamed `subModel` because it’s more clear, and consistent with the new `subModelOpt` and `subModelSeq`
* `Program.runDebugWindow` has been removed in favour of `Program.runWindowWithConfig`
* Bundled Elmish has been removed, and Elmish 2.0 is used as an external dependency
* Any `Application ` instance instantiated before calling `Program.run...` will now be used
* Several new functions in the `Binding` module; dot into it in your IDE or see the repository for samples or source code

#### 1.0.0-beta-7

* Fix for #19, model to view updates for validation bindings

#### 1.0.0-beta-6

* Implemented INotifyDataErrorInfo and corresponding bindings
* Added some documentation for binding assemblers
* Added message box error handler to Program module

#### 1.0.0-beta-5

* Target F# 4.1
* Lastest fable-elmish, includes memory leak fix

#### 1.0.0-beta-4

* Added Program.withExceptionHandler

#### 1.0.0-beta-3

* Fixing nuget framework version

#### 1.0.0-beta-2

* Added command parameter
* Renamed Binding.vm to Binding.model
* Reorganized samples and added performance sample (WIP)

#### 1.0.0-beta-1

* Fixing two way binding bugs

#### 0.9.0-beta-9

* Elmish all the WPF!
