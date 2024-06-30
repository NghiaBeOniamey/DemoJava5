# Hướng dẫn sử dụng Sourcetree

## Mục lục

- [Giới thiệu](#giới-thiệu)
- [Yêu cầu hệ thống](#yêu-cầu-hệ-thống)
- [Cài đặt](#cài-đặt)
- [Sử dụng](#sử-dụng)
- [Pull Request](#pull-request)
- [Resolve Conflict](#resolve-conflict)
- [Command Line Bổ Sung](#command-line-bổ-sung)
- [Liên hệ](#liên-hệ)

## Giới thiệu

Đây là cách thôi sử dụng git cùng nhóm.

## Yêu cầu hệ thống

Tôi đang sự dụng hệ điều hành windows và tool Sourcetree tích hợp cho MacOS và Windows.

- System: MacOS, Windows.
- Git: Khuyến nghị version mới nhất.
- Sourcetree: Sử dụng cả terminal và tool để tiết kiệm thời gian.
- Account Bitbucket: Support tốt hơn cho git.

### Git Version

Hãy tham khảo Makedown sau: [_setup.md_](/README.setup.md)

## Cài đặt

### Sourcetree & Bitbucket

Hãy tham khảo các tài liệu sau:

- **[_Download & Setup_](https://www.geeksforgeeks.org/how-to-install-sourcetree-for-git-in-windows/)**

- **[_Bitbucket Support & Sourcetree Tutorial_](https://support.atlassian.com/bitbucket-cloud/docs/tutorial-learn-bitbucket-with-sourcetree/)**

## Sử dụng

### Create Repository

1. Đăng nhập [GitHub](https://github.com/)

2. Truy cập vào [GitHub](https://github.com/new)

   ![CreateRepo](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/GitHub/create-repo.png)

### Sourcetree Create Repo & Push, Fetch Code & Get Code Basics

1. Clone repository

   ![CloneRepo](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/Sourcetree/clone-repo.png)

2. Create branch

   ![CreateBranch](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/Sourcetree/create-branch.png)

3. Create file and code some thing

   ![CreateFileAndCoding](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/Sourcetree/create-code-index.html.png)

4. Stage file and commit code

   ![StageAndCommitCode](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/Sourcetree/stage-commit.png)

5. Push code to remote

   | Old Code                                                                                                                        | New Code                                                                                                                        |
   | ------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
   | ![OldCode](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/Sourcetree/old-code.png) | ![NewCode](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/Sourcetree/new-code.png) |

   | Push Code                                                                                                                         |
   | --------------------------------------------------------------------------------------------------------------------------------- |
   | ![PushCode](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/Sourcetree/push-code.png) |

   | Old Remote                                                                                                                          | New Remote                                                                                                                          |
   | ----------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
   | ![OldRemote](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/Sourcetree/old-remote.png) | ![NewRemote](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/Sourcetree/new-remote.png) |

   > Note: you need Discard All File Change or Commit Your Code Before Pull, Checkout `another || new` branch on remote😎.

6. Get code on remote to local(Fetch Code)

   | Fetch Code                                                                                                                          | Pull Code                                                                                                                         |
   | ----------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
   | ![FetchCode](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/Sourcetree/fetch-code.png) | ![PullCode](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/Sourcetree/pull-code.png) |

7. Get code local to your branch(Fetch Code and Checkout)

   | `st_1` Fetch To Update Local `st_2` Pull Code To Get Code Local to your branch or Checkout new branch on remote branch                            |
   | ------------------------------------------------------------------------------------------------------------------------------------------------- |
   | ![GetCodeOnRemote](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/Sourcetree/get-code-on-remote.png) |

## Pull Request

> 🙏🏻Pls Recommended Use Github Remote To Create Pull Request And Resolve Conflict On Local Alter Push Your Code

1.  Push your code to remote.
2.  Access https://github.com/`AccountName`/`RepoName`: **[_My Example_](https://github.com/NghiaBeOniamey/NewRepo)**.
3.  Create pull request.

    | `For All Cases` Your can skip suggess pull and click `Pull Request`                                                                                 |
    | --------------------------------------------------------------------------------------------------------------------------------------------------- |
    | ![ClickPullRequestForAllCases](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/GitHub/pull-request.png) |

    | `For All Cases` Your can skip suggess pull and click `New Pull Request`                                                                    |
    | ------------------------------------------------------------------------------------------------------------------------------------------ |
    | ![NewPullRequest](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/GitHub/new-pull-request.png) |

    | `For All Cases` Your can skip suggess pull and click `Your branch has just been pushed`                                                   |
    | ----------------------------------------------------------------------------------------------------------------------------------------- |
    | ![YourBranchJustPush](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/GitHub/your-branch.png) |

    > You need check ( your branch have pull to where )

    | `Check` branch, file change, commit code alter and press Create Pull Request                                                            |
    | --------------------------------------------------------------------------------------------------------------------------------------- |
    | ![Checking](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/GitHub/create-pull-request.png) |

    | Add A Description You Had Code On Your Branch                                                                                             |
    | ----------------------------------------------------------------------------------------------------------------------------------------- |
    | ![AddDescription](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/GitHub/add-description.png) |

    > Success

    | Call Your Lead Wait Your TeachLeader Review, Authorization Your Pull Request                                              |
    | ------------------------------------------------------------------------------------------------------------------------- |
    | ![Success](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/GitHub/sucess.png) |

> Faster

1.  Push your code to remote.
2.  Access https://github.com/`AccountName`/`RepoName`/compare: **[_My Example_](https://github.com/NghiaBeOniamey/NewRepo/compare)**.
3.  Create pull request
    | `For All Cases` Your can skip suggess pull and click `Your branch has just been pushed` |
    | --------------------------------------------------------------------------------------- |
    | ![YourBranchJustPush](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/GitHub/your-branch.png) |

    > You need check ( your branch have pull to where )

    | `Check` branch, file change, commit code alter and press Create Pull Request                                                            |
    | --------------------------------------------------------------------------------------------------------------------------------------- |
    | ![Checking](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/GitHub/create-pull-request.png) |

    | Add A Description You Had Code On Your Branch                                                                                             |
    | ----------------------------------------------------------------------------------------------------------------------------------------- |
    | ![AddDescription](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/GitHub/add-description.png) |

    > Success

    | Call Your Lead Wait Your TeachLeader Review, Authorization Your Pull Request                                              |
    | ------------------------------------------------------------------------------------------------------------------------- |
    | ![Success](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/GitHub/sucess.png) |

## Resolve Conflict

### Merge Code

1. Can't automatically merge

   | Can't automatically merge        |
   | -------------------------------- |
   | ![WarningPullRequest](/Learn/git/git-tutorial/images/GitHub/can't-automatically-merge.png) |

2. Use sourtree

   > Step 1

   Fetch code. >[How to fetch code with Sourcetree](#sourcetree-create-repo--push-fetch-code--get-code-basics)

   > Step 2

   ```
   > Note:

   1. You can't delete your current branch.

   2. You need commit your code alter delete or checkout branch.

   3. In this example i trying pull request to dev [ Resolve Conflict with VS Code, Intellij Idea ].
   ```

   | Delete branch you wan't create pull request on side bar Branches. |
   | ----------------------------------------------------------------- |
   | ![Delete](/Learn/git/git-tutorial/images/Sourcetree/resolve-conflig-delete-branch.png)                                          |

   | Checkout new branch on remote. |
   | ------------------------------ |
   | ![Checkout](/Learn/git/git-tutorial/images/Sourcetree/resolve-confilg-checkout-branch.png)       |

   | Merge branch into current branch. <div>Must checkout your branch you want create pull request before.</div> |
   | ----------------------------------------------------------------------------------------------------------- |
   | ![Merge](/Learn/git/git-tutorial/images/Sourcetree/resolve-confilg-merge-into-current-branch.png)                                                                                    |

### Resolve Conflict

1. VS Code

   ````
      > Select file conflig
   ````

   |  Resolve In Merge Editor  |
   | -------------------------------- |
   | ![SelectFileResolve](/Learn/git/git-tutorial/images/VSCode/select-file-resolve.png) |

   |  Resolve In Merge Editor  |
   | -------------------------------- |
   | ![UIUXMergeEditor](/Learn/git/git-tutorial/images/VSCode/UIUX-MergeEditor.png) |

   ````
   > Select Option And Check Resuilt:

   1. Accept Incoming: Chấp nhận thay đổi.

   2. Accept Combination: Chấp nhận cả 2 thay đổi.

   ````

   |  Resolve In Merge Editor Click Merge Code |
   | -------------------------------- |
   |    ![Resuilt](/Learn/git/git-tutorial/images/VSCode/resuilt-merge.png) |

   ````
      > Alter resolve all conflig, you can commit, push code and create pull request.
   ````

2. IntelliJ IDEA

   ````
   > Select file conflig
   ````

   |  Resolve In Merge Editor  |
   | -------------------------------- |
   | ![SelectFileResolve](/Learn/git/git-tutorial/images/IntellijIdea/select-file-resolve.png) |

   |  Resolve In Merge Editor  |
   | -------------------------------- |
   | ![UIUXMergeEditor](/Learn/git/git-tutorial/images/IntellijIdea/UIUX-MergeEditor.png) |

   ````
   > Select Option And Check Resuilt:

   1. Accept Incoming: Chấp nhận thay đổi.

   2. Accept Combination: Chấp nhận cả 2 thay đổi.

   ````

   |  Resolve In Merge Editor Click Apply |
   | -------------------------------- |
   |    ![Resuilt](/Learn/git/git-tutorial/images/IntellijIdea/resuilt-merge.png) |

   ````
   > Alter resolve all conflig, you can commit, push code and create pull request.
   ````

## Command Line Bổ Sung

![GitBasicsComandLineTerminal](https://github.com/NghiaBeOniamey/MarkdownExample/blob/master/Learn/git/git-tutorial/images/use/git-basics.png)

- `git init` tạo một kho Git trong thư mục cục bộ.

- `git clone` <remote-repo-address>: sao chép toàn bộ kho từ máy chủ từ xa đến thư mục cục bộ. Bạn cũng có thể sử dụng nó để sao chép kho cục bộ.

- `git add` <file.txt>: thêm một tệp hoặc nhiều tệp và thư mục vào khu vực tạm thời.

- `git commit -m "Thông điệp"`: tạo một bản chụp nhanh của các thay đổi và lưu nó vào kho. [ **[_cheat-sheet_](https://www.conventionalcommits.org/en/v1.0.0/)** & **[_fast-example_](/README.gitcommit.md)** ]

- `git config` được sử dụng để thiết lập cấu hình cụ thể của người dùng như email, tên người dùng và định dạng tệp.

- `git status` hiển thị danh sách các tệp đã thay đổi hoặc các tệp chưa được thêm vào khu vực tạm thời và cam kết.

- `git push <remote-name> <branch-name>`: gửi các cam kết cục bộ lên nhánh từ xa của kho.

- `git checkout -b <branch-name>`: tạo một nhánh mới và chuyển sang nhánh mới đó.

- `git remote -v` xem tất cả các kho từ xa.

- `git remote add <remote-name> <host-or-remoteURL>`: thêm máy chủ từ xa vào kho cục bộ.

- `git branch -d <branch-name>`: xóa nhánh.

- `git pull` hợp nhất các cam kết vào thư mục cục bộ từ kho từ xa.

- `git merge <branch-name>`: sau khi giải quyết xung đột hợp nhất, lệnh này sẽ pha trộn nhánh đã chọn vào nhánh hiện tại.

- `git log` hiển thị danh sách chi tiết các cam kết cho nhánh hiện tại.

## Liên hệ

Nếu bạn có bất kỳ câu hỏi nào, vui lòng liên hệ qua email [nghiabe.dev@gmail.com].
