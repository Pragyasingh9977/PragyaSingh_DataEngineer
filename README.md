# PragyaSingh_DataEngineer
from typing import List


class Int:
    name: str
    text: str

    def __init__(self, name: str, text: str) -> None:
        self.name = name
        self.text = text


class LstLst:
    lst_str: List[Int]
    name: str

    def __init__(self, lst_str: List[Int], name: str) -> None:
        self.lst_str = lst_str
        self.name = name


class ResponseLst:
    lst_int: List[Int]
    lst: LstLst
    name: str

    def __init__(self, lst_int: List[Int], lst: LstLst, name: str) -> None:
        self.lst_int = lst_int
        self.lst = lst
        self.name = name


class Doc:
    doc_str: List[Int]
    date: List[Int]
    long: Int

    def __init__(self, doc_str: List[Int], date: List[Int], long: Int) -> None:
        self.doc_str = doc_str
        self.date = date
        self.long = long


class Result:
    doc: List[Doc]
    name: str
    num_found: int
    start: int

    def __init__(self, doc: List[Doc], name: str, num_found: int, start: int) -> None:
        self.doc = doc
        self.name = name
        self.num_found = num_found
        self.start = start


class Response:
    lst: ResponseLst
    result: Result

    def __init__(self, lst: ResponseLst, result: Result) -> None:
        self.lst = lst
        self.result = result


class Welcome8:
    response: Response

    def __init__(self, response: Response) -> None:
        self.response = response
