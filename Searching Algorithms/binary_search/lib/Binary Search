class Searching {
  int? binarySearch(List<int> nums, target) {
    int l = 0;
    int r = nums.length - 1;
    while (l <= r) {
      int mid = l + (r - l) ~/ 2;
      if (nums[mid] == target) return mid;
      if (nums[mid] < target)
        l = mid + 1;
      else
        r = mid - 1;
    }
    return -1;
  }
}

void main(List<String> arguments) {
  Searching searching = Searching();
  List<int> nums = [1, 2, 4, 5, 7];
  int target = 0;
  print(searching.binarySearch(nums, target));
}
