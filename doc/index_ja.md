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
