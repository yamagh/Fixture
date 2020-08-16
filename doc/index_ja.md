# Documentation

## Getting Started

### Basic Usage

## Actions

### Fixture_Setup

テスト用テナントのセットアップを行う。

次のセットアップを行う:

- テスト用テナントを作成し現在のコンテキストを切り替える。デフォルトのテナントの名前は 'Fixture'。
- テスト用ユーザを作成しログインする。デフォルトのユーザ名は 'FixtureRunner'。
- テストデータの指定がある場合は、そのデータをテスト用テナントにインポートする。

#### Properties

##### TestData: YAML フォーマットのテストデータ

例:

```YAML
ModuleName:
  EntityName1:
    Record1:
      Id: &record1
      Attr: foo
  EntityName2:
    Record2:
      Id: *record1
      Attr: bar
```

### Fixture_Teardown

テストデータの破棄を行う

マルチテナントのエンティティの中のデータを削除する。シングルテナントの中のデータは削除されない事に注意してください。

#### Properties

無し

## YAML for Fixture

Fixture で利用可能な YAML のフォーマットについて記載する。

## Advanced Guide

## Q&A

### 1. ランダムな値を使用したい

次の Froge のコンポーネントが役に立ちます。

- [Randomizer Number Generator](https://www.outsystems.com/forge/component-overview/677/randomizer-number-generator)
- [RandomInteger - Overview - OutSystems](https://www.outsystems.com/forge/component-overview/1836/randominteger)
- [Random Number List Generator - Overview - OutSystems](https://www.outsystems.com/forge/component-overview/2761/random-number-list-generator)
- [RandomClass - Component Versions - OutSystems](https://www.outsystems.com/forge/component-versions/1474)
